## RecruitOn 

<p align="center">
  <img src="https://github.com/ims-opensolutions/space-frog-recruit-on-app/blob/master/logo/Recruit0n_big.jpg" width=500 alt="RecruitOn Logo" />
</p>

<p align="center">A web application to handle and process an organization's candidates data</p>

## Description

<p align="justify">RecruitOn is a humble web application which aims to ease the process of handling, filtering and organizing potential candidates personal data. Target here is actually any organization or company that deals with recruiting processes (normally HHRR team). It works resorting on a simple UI which allows the user to upload an excel file. The logic behind the application process this data and shows it back to the client in a user-friendly way. </p>

<p align="justify">The application offers some interesting functions. Among them, we have:</p>

* <p>Filtering through different parameters: qualification, salary and location</p>
* <p>Ubicate the candidate in a map</p>

## Features

<p align="justify">Most important, remarkable feature regarding UX is a custom handling of browser navigation history</p>

## Tools

* <p>Chrome Web Request API</p>
* <p>JavaScript History API</p>
* <p>JavaScript Web Crypto API</p>
* <p>Let's Encrypt certificates</p>

## Security

<p align="justify">From its very early birth stage, RecruitOn was thought to be build and constructed in the most secure possible way, giving thus to this factor a top priority. For this to be achieved, a different approach from traditional user-password login mechanism was desired. The main goal was authenticating requestes made by RecruitOn, accepting only them and rejecting any other one coming from a different source.</p>

<p align="justify">The core of the security RecruitOn engine has been finally set up throuhg Chrome Web Request API. In a simplified explanation, this API works by installing an extension on chrome, which intercepts any requests coming from the application. Next, it encrypts a given payload that is sent to the server in hexadecimal format, which will be responsible for decrypting this data and validating it.</p>

<p align="justify">A second security layer has been configured through short-live cookies. These are triggered on onbeforeunload JavaScript native event, allowing the client to  create them only when the next request is about to be launched. This shortens up the time the cookie is present in the browser. In addition, the lifetime of the cookie is just 2 seconds. Then, it the browser purges it. To assure a background layer against potential CSRF attacks, samesite attribute is also set along the rest of the cookie properties.</p>

<p align="justify">Finally, all the traffic is encrypted even in development phase. This has been done with self-certified https credentials provided by Let's Encrypt.</p>

## Versions

* <p>1.0</p>

## License

<p align="justify">All rights reserved to MKNA security software development.</p>

