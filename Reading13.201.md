## In today's reading  we learn the importance of storage ##

### *Why would a developer use local storage for a web application?* ###

- The main problem with HTTP as the main transport layer of the Web is that it is stateless. This means that when you use an application and then close it, its state will be reset the next time you open it. If you close an application on your desktop and re-open it, its most recent state is restored.


### *What information should not be stored in local storage?* ###

- Because cookies have been used to spy on people’s surfing behavior, security-conscious people and companies turn them off or request to be asked every time whether a cookie should be set.

### *Local storage can store what type of data? How would you convert it to that type before storing?* ###

- Using local storage in modern browsers is ridiculously easy. All you have to do is modify the localStorage object in JavaScript. You can do that directly or (and this is probably cleaner) use the setItem() and getItem() method. One annoying shortcoming of local storage is that you can only store strings in the different keys. This means that when you have an object, it will not be stored the right way.


(Reference: Smashing Magazine)

## Things I want to know more about 

- None for now