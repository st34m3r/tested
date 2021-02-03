# tested

open postman</br>  
create new POST request</br>
url =<wsdl url> // http://localhost:8080/holidayService</br>
in the header section add :</br>
  Content-Type = text/xml; charset=UTF-8</br>

# raw test body 
```xml
<?xml version="1.0" encoding="ISO-8859-1" standalone="no"?>
<test>
  <value>ácentó y la letra ñ<value>
</test>
```

this print a message in the debug console :</br>
  Booking holiday for [{Thu Jan 22 00:00:00 GMT+01:00 2004} - {Fri Jan 15 00:00:00 GMT+01:00 2021}] for [{Name lastname}]</br> 
