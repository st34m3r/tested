# tested

open postman</br>  
create new POST request</br>
url =<wsdl url> // http://localhost:8080/holidayService</br>
in the header section add :</br>
  Content-Type = text/xml; charset=UTF-8</br>

# raw test body 
</br>
```xml
<myxml>
   <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:sch="http://joedayz.pe/hr/schemas"></br>
   <soapenv:Header/></br>
    <soapenv:Body></br>
      <sch:HolidayRequest></br>
         <sch:Holiday></br>
            <sch:StartDate>2004-01-22</sch:StartDate></br>
            <sch:EndDate>2021-01-15</sch:EndDate></br>
         </sch:Holiday></br>
         <sch:Employee></br>
            <sch:Number>15</sch:Number></br>
            <sch:FirstName>name</sch:FirstName></br>
            <sch:LastName>lastname</sch:LastName></br>
         </sch:Employee></br>
      </sch:HolidayRequest></br>
   </soapenv:Body></br>
</soapenv:Envelope></br> 
</myxml>
```


this print a message in the debug console :</br>
  Booking holiday for [{Thu Jan 22 00:00:00 GMT+01:00 2004} - {Fri Jan 15 00:00:00 GMT+01:00 2021}] for [{Name lastname}]</br> 
