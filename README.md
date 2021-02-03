# tested

open postman  
create new POST request 
url =<wsdl url> // http://localhost:8080/holidayService
in the header section add : 
  Content-Type = text/xml; charset=UTF-8

# raw test body 

<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:sch="http://joedayz.pe/hr/schemas">
   <soapenv:Header/>
    <soapenv:Body>
      <sch:HolidayRequest>
         <sch:Holiday>
            <sch:StartDate>2004-01-22</sch:StartDate>
            <sch:EndDate>2021-01-15</sch:EndDate>
         </sch:Holiday>
         <sch:Employee>
            <sch:Number>15</sch:Number>
            <sch:FirstName>name</sch:FirstName>
            <sch:LastName>lastname</sch:LastName>
         </sch:Employee>
      </sch:HolidayRequest>
   </soapenv:Body>
</soapenv:Envelope>


this print a message in the debug console :
  Booking holiday for [{Thu Jan 22 00:00:00 GMT+01:00 2004} - {Fri Jan 15 00:00:00 GMT+01:00 2021}] for [{Name lastname}] 