# OpenWeatherTestApp
This is a java test application for the http://openweathermap.org/ site.

- Here are some test cases I came up with,  trying to include different scenarios I thought are useful for web applications that share "Restful" web services.

Class with Test Cases: OpenWeatherTest.java

* Verify we can retrieve the name of the City we are interested in, by specifying its Id.
  Method: testGetCityNameById()

* Validate that we cannot get the name of a city in case we don´t provide a correct Id. 
  Method: testNegativeGetCityNameById()

* Validate that based on different Ids (stored in a resource file with a list), we are able to get different parameters for each entry provided in the list file.
  Method: testGetAllCitiesById()

* Validate the response code is OK (200), when we provide a valid zip code. Also it validates we are able to retrieve the coordinates for that zipcode.
  Method: testWeatherDataByZipCode()

* Validate we receive a Unauthorized code (401) when we provide an invalid uri.
  Method: testBadRequest()

* Verify that Response Headers are what we expect.
  Method: testReturnedHeaders()
