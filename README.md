# tested

open postman</br>  
create new POST request</br>
url =<wsdl url> // http://localhost:8080/holidayService</br>
in the header section add :</br>
  Content-Type = text/xml; charset=UTF-8</br>

# raw test body 
```xml
<?xml version="1.0" encoding="ISO-8859-1" standalone="no"?>
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:sch="http://joedayz.pe/hr/schemas">
   <soapenv:Header/>
    <soapenv:Body>
      <sch:HolidayRequest>
         <!--You may enter the following 2 items in any order-->
         <sch:Holiday>
            <sch:StartDate>2004-01-22</sch:StartDate>
            <sch:EndDate>2021-01-15</sch:EndDate>
         </sch:Holiday>
         <sch:Employee>
            <sch:Number>15</sch:Number>
            <sch:FirstName>Omar</sch:FirstName>
            <sch:LastName>Imai</sch:LastName>
         </sch:Employee>
      </sch:HolidayRequest>
   </soapenv:Body>
</soapenv:Envelope>
```

this print a message in the debug console :</br>
  Booking holiday for [{Thu Jan 22 00:00:00 GMT+01:00 2004} - {Fri Jan 15 00:00:00 GMT+01:00 2021}] for [{Name lastname}]</br> 
