# PDF.js [![Build Status](https://github.com/mozilla/pdf.js/workflows/CI/badge.svg?branch=master)](https://github.com/mozilla/pdf.js/actions?query=workflow%3ACI+branch%3Amaster)

Versión de PDF.js modificada para externalizar dos funciones con el proposito de desencriptar streams en pdfs con contraseña de usuario vacía.

# Funciones
* pdfDoc.decStream(obj,gen,stream) 
        
        ( UInt8Array -> UInt8Array )
    Nos permite desencriptar un stream. Es necesario pasar la referencia(Object number y generation number) del stream, ya que se usan para la desencriptación. 
#    

* pdfDoc.getXEntries()
        
        ( Array )
    Nos devuelve la tabla de Xref, con los bytes de inicio y generation numbers de cada objeto. 

#