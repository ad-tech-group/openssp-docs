## OpenSSP by One tech Group

### This is an open-source supply-side platform for general use with full OpenRTB support.

OpenSSP is a so-called multi-channel SSP which means that not only does it support RTB, but also channels to ad server and further SSP implementation. The RTB support is a core feature and needs no extra definition.

OpenSSP supports the power of the OpenRTB standard, and can be used to deliver banner impressions, videoad impressions etc.
Feel free to examine the code and modify it as you need.


![OpenSSp RTB Ecosystem](assets/openssp-eco.png)

### General SSP Functionality:
- A tag with a link to OpenSSP needs to be placed on a website that contains the ad placement. This link may contain a set of parameters (depending on your preferences). 
- OpenSSP is then called from the tag and the parameters are extracted and validated.
- OpenSSP resolves the request data, e.g. the website or publisher which is identified by an ID and loads additional data from cache (more information on data caching).
- OpenSSP starts the ExchangeServer and the ExecutorService to call a demand service (DSP, SSP, Adserver etc.) and waits for the response to start the auction.
- After the auction is finished, the winner is evaluated and a response to the client will be sent.

Feel free to use the code, modify it and improve it!

Comments, proposals and suggestions are welcome.

OTG, May 2017.
