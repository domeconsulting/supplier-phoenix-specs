## ExtraCustomData
> Detalle del elemento ExtraCustomData del mensaje BookingRetrieval. 

````xml
<?xml version="1.0" encoding="UTF-8"?>
<BookingRetrievalResponse>
    <sessionId>SUP#FOO#123456789</sessionId>
    <booking>
	   ...
	   <extraCustomData>
          <customData>
             <key>Key1</key> 
             <value>Value1</value>
           </customData>
           <customData>
              <key>Key2</key>
              <value>Value2</value>
           </customData>
       </extraCustomData>
    </booking>
</BookingRetrievalResponse>
````

````json
{
  "BookingRetrievalResponse": {
    "sessionId": "SUP#FOO#123456789",
    "booking": {
	  ... 	
      "extraCustomData": {
        "customData": [
          {
            "key": "Key1",
            "value": "Value1"
          },
          {
            "key": "Key2",
            "value": "Value2"
          }
        ]
      }
    }
  }
}
````

Elemento **Opcional** utilizado para indicar diversos aspectos de la reserva que no tienen cabida en el formato básico de la reserva. 

**Solo se notificarán aquellos elementos que estén informados.**


### CustomData Keys

A continuación se detallan los distintos valores que pueden llegar en el elemento key.
 
Key | Tipo |  Descripción
--------- | ----------- | -----------
LastMinute | S / N (Si/No) | Indica si se trata de una reserva realizada a traves del componente LastMinute de la web
SEMCODE | *String* | Indica el código de SEM 
BookingEngineCode | *Integer* | Indica el código de motor de la web
WebsiteUrl | *String* | Indica la url de la web donde se ha realizado la reserva.
IpAdress | *String* | Indica la ip desde la cual se ha realizado la reserva.
Country | *String* | Indica el pais desde el cual se ha realizado la reserva. (ISO 3166)
ReferredByUrl | *String* | Indica la Url desde la cual ha llegado la reserva.
ReferredBySystem | *String* | Indica el sistema desde el cual ha llegado la reserva. (GHF -Google Hotel Finder-, TVG -Trivago-).
Affiliate | *String* | 
Medium | *String* |
Source | *String* |

