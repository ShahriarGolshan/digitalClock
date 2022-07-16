# digitalClock

### Installation

First we need to add this js file as external references 

	<script src="/js/digitalClock.js"></script>
  
  
  
#### Download .zip

[Download .ZIP](https://github.com/ShahriarGolshan/digitalClock/raw/main/DigitalClock.rar)

---

### Documentation

after adding digitalClock.js file to the html you can start using this script

	const digitalClock = new DigitalClock({
      containerElement: document.querySelector("#digital-clock")
	});

next

    digitalClock.init();
    digitalClock.createClock();
    
#### Options

##### set custom date
You can insert an ISOString to when useing createClock function to use your own date

	const customeDate = new Date(2001,3,21,12,59,57);
    customeDate.toISOString();
    digitalClock.createClock(customeDate)


##### set twelveHourFormat
You can pass an option to DigitalClock object to use 12 hour formated clock

	const digitalClock = new DigitalClock({
      ...
      twelveHourFormat: true,
      ...
	});
  
  
##### showing twelveHourFormat period AM/PM
You can pass an option to DigitalClock object to use 12 hour formated clock

	const digitalClock = new DigitalClock({
      ...
      twelveHourFormat: true,
      periodElement: document.querySelector("#digital-clock__period"),
      ...
	});
  
  
##### disabledPeriod
You can pass an option to DigitalClock object to disabled period and it will not show up

	const digitalClock = new DigitalClock({
      ...
      twelveHourFormat: true,
      disabledPeriod: true,
      containerElement: document.querySelector("#digital-clock"),
      ...
	});
  
  
##### showing clock in targeted node
You can pass an option to DigitalClock object to use clock in your custom element

	const digitalClock = new DigitalClock({
      clockElement: document.querySelector(".digital-clock__clock")
	});
  
  
##### custom class name
You can pass an option to DigitalClock object to use your class name

	const digitalClock = new DigitalClock({
      ...
      className: "custom",
      ...
	});
  
