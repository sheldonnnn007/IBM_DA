# APIs, and Data Collection

## Simple APIs

**Keys** will give authorizetion to access the source

Application Program Interface (API):

#### What is an API

![image-20230322105411437](./photo/image-20230322105411437.png)

#### API Libraries

#### Rest API

- Request and Response

  **RE**presentional **S**tate **T**ransfer APIs

  ![image-20230322110753117](./photo/image-20230322110753117.png)

  

- An Example with PyCoinGecko

## REST APIs, Webscraping, and Working with Files

- Uniform Resource Locator: URL

HTTP: a general protocol of transferring information through the web

The <u>request</u> be send by API communicates via HTTP message.

> Scheme: the protocol, Http://
>
> Internet address or Base URL: www.ibm.com
>
> Route: /images/IDSlogo.png
>
> - http://www.ibm.com/images/IDSNlogo.png

- Request

  Import requests

  

- Response

#### Webscraping

Find_all

All kinds of file formats

- CSV: pandas: df.read_csv("...")

- JSON: import json: 

  ![image-20230322145933776](./photo/image-20230322145933776.png)

- XML: 

  ![image-20230322150114276](./photo/image-20230322150114276.png)

  ![image-20230322150148030](./photo/image-20230322150148030.png)



#### Beautiful soup

 **represents the document as a nested data structure**
soup = BeautifulSoup(html, "html.parser")

print(soup.prettify())![image-20230323103700057](./photo/image-20230323103700057.png)

tag_object=soup.title
print("tag object type:",type(tag_object))![image-20230323103845681](./photo/image-20230323103845681.png)
tag object type: <class 'bs4.element.Tag'>

![image-20230323104108880](./photo/image-20230323104108880.png)
tag_object.parent
tag_object.next_sibling

![image-20230323104233918](./photo/image-20230323104233918.png)
![image-20230323104314210](./photo/image-20230323104314210.png)
![image-20230323104521779](./photo/image-20230323104521779.png)



#### Navigable String
![image-20230323104802967](./photo/image-20230323104802967.png)
unicode_string = str(tag_string)





#### Filter

![image-20230323104939581](./photo/image-20230323104939581.png)

<table>
  <tr>
    <td id='flight' >Flight No</td>
    <td>Launch site</td> 
    <td>Payload mass</td>
   </tr>
  <tr> 
    <td>1</td>
    <td><a href='https://en.wikipedia.org/wiki/Florida'>Florida</a></td>
    <td>300 kg</td>
  </tr>
  <tr>
    <td>2</td>
    <td><a href='https://en.wikipedia.org/wiki/Texas'>Texas</a></td>
    <td>94 kg</td>
  </tr>
  <tr>
    <td>3</td>
    <td><a href='https://en.wikipedia.org/wiki/Florida'>Florida<a> </td>
    <td>80 kg</td>
  </tr>
</table>

![image-20230323105235024](./photo/image-20230323105235024.png)



#### find All

table_rows=table_bs.find_all('tr')  --(extract all the tags with that name and its children.)

first_row =table_rows[0]

![image-20230323105850966](./photo/image-20230323105850966.png)







<h3>Rocket Launch </h3>

<p>
<table class='rocket'>
  <tr>
    <td>Flight No</td>
    <td>Launch site</td> 
    <td>Payload mass</td>
  </tr>
  <tr>
    <td>1</td>
    <td>Florida</td>
    <td>300 kg</td>
  </tr>
  <tr>
    <td>2</td>
    <td>Texas</td>
    <td>94 kg</td>
  </tr>
  <tr>
    <td>3</td>
    <td>Florida </td>
    <td>80 kg</td>
  </tr>
</table>
</p>
<p>

<h3>Pizza Party  </h3>


<table class='pizza'>
  <tr>
    <td>Pizza Place</td>
    <td>Orders</td> 
    <td>Slices </td>
   </tr>
  <tr>
    <td>Domino's Pizza</td>
    <td>10</td>
    <td>100</td>
  </tr>
  <tr>
    <td>Little Caesars</td>
    <td>12</td>
    <td >144 </td>
  </tr>
  <tr>
    <td>Papa John's </td>
    <td>15 </td>
    <td>165</td>
  </tr>

![image-20230323110943601](./photo/image-20230323110943601.png)



![image-20230323111605221](./photo/image-20230323111605221.png)

soup = BeautifulSoup(data,"html.parser")

![image-20230323111714344](./photo/image-20230323111714344.png)

![image-20230323111748904](./photo/image-20230323111748904.png)

![image-20230323111935992](./photo/image-20230323111935992.png)



### Table

![image-20230323112854652](./photo/image-20230323112854652.png)

![image-20230323112233886](./photo/image-20230323112233886.png)

![image-20230323112304771](./photo/image-20230323112304771.png)

![image-20230323112506681](./photo/image-20230323112506681.png)

![image-20230323113551923](./photo/image-20230323113551923.png)





**BeautifulSoup**

![image-20230323113811070](./photo/image-20230323113811070.png)





![image-20230323113957036](./photo/image-20230323113957036.png)
