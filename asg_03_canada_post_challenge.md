# Assignment 03: Getting Iffy with It

## Canada Post Challenge

_Mail Time!_

---

_I had to send a package recently to a friend in Grande Prairie. Brought the thing up to the counter and it was weighed, measured, stickered and placed with care into the loving arms of our national postal service. I said to myself, "Self - this would make a helluva good coding challenge!" Lucky you._

_After digging around a bit on the Canada Post site, I found [this document](https://www.canadapost.ca/tools/pg/prices/CPprices-e.pdf) that has the Canada Post prices for 2017. On page 5, it basically says to calculate a shipping price, you need to:_

1. "Find the applicable rate code for your packages origin and destination."
1. "Refer to your price sheets to determine the shipping price according to the apppropriate [sic] rate code, weight and service."

_Since making a full-blown price calculator is **way** beyond cruel, we're going to something more stripped down: a little app that, when given the dimensions and weight of a package, tells you what row to look up in the Regular Parcel Prices table (starting on page 10 in the price doc mentioned earlier). And it will give you something called the Forward Sortation Area as well._

_Here are some assumptions we'll make:_

* All packages are regular box-shaped packages. No tubes, triangular prisms, or abstract sculptures.
* All packages will be sent via **Regular Parcel** service.
* We don't need to worry about oversized or overweight packages.

---

**MAKE THIS HAPPEN:**

Write code that does the following:

1. Prompts the user for and obtains the width of the package in cm.
    * You may assume the user enters a valid positive number. This number may have a decimal.
1. Prompts the user for and obtains the height of the package in cm.
    * You may assume the user enters a valid positive number. This number may have a decimal.
1. Prompts the user for and obtains the length of the package in cm.
    * You may assume the user enters a valid positive number. This number may have a decimal.
1. Prompts the user for and obtains the weight of the package in kg.
    * You may assume the user enters a valid positive number. This number may have a decimal.
1. Prompts the user for and obtains the destination postal code.
    * You may assume that the user enters a postal code...but they may forget the space and/or forget to capitalize everything.
1. Outputs one of the two following sentences:
    * `The shipping charge will be based on package weight.`
    * `The shipping charge will be based on the volumetric equivalent of weight.`
    * You **must** include these sentences **exactly** as written, or the automated tests will fail!
1. Outputs the weight row to use in the price sheet for regular parcels.
    * For example, "Look up weight row 10.5."
    * The automated tests only care about the number for this output. The format of these numbers must match what you see in the first column of the Regular Parcel Prices table.
1. Outputs the first 3 characters of the destination's postal code - this is called the _Forward Sortation Area (FSA)_. (This would be used by the user of the app to figure out what column in the table to use.)
    * For example, `Forward Sortation Area: T3E`
    * The automated tests need the FSA to be in all caps.

**NOTES:**
1. You'll have to read section 3.4 (_Shipping charges and weight_) of Canada Post's [ABCs of Mailing](https://www.canadapost.ca/tools/pg/manual/PGabcmail-e.asp) on how to calculate the volumetric equivalent of actual weight.
1. From the same section, notice that when calculating your weight row, you need to round "to the nearest 0.500". But in the price tables given, prices are rounded to the nearest 0.5, so we'll use that instead.
1. Also from the same section, notice that the minimum weight/VE row possible is 0.75...this is different from the other rows, where you're rounding to the nearest 0.5. You have to deal with this.
1. If the package weight and VE equivalent of weight are the same, then the shipping charge should be based on package weight.

