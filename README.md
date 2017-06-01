## OpenSSP by ATG

### This is an open-source supply-side platform for general use with full OpenRTB support.

OpenSSP is a so-called multi-channel SSP which means that not only does it support RTB, but also channels to ad server and further SSP implementation. The RTB support is a core feature and needs no extra definition.

This SSP is specifically optimized for handling video ad impressions, but it can also be used for any other type of ad impressions such as display etc. Feel free to examine the code and modify it as you need.

### General SSP Functionality:
1. A tag with a link to OpenSSP needs to be placed on a website that contains the ad placement. This link may contain a set of parameters (depending on your preferences). 
2. OpenSSP is then called from the tag and the parameters are extracted and validated.
3. OpenSSP resolves the request data, e.g. the website or publisher which is identified by an ID and loads additional data from cache (more information on data caching).
4. OpenSSP starts the ExchangeServer and the ExecutorService to call a demand service (DSP, SSP, Adserver etc.) and waits for the response to start the auction.
5. After the auction is finished, the winner is evaluated and a response to the client will be send.

Feel free to use the code, modify it and improve it!

Comments, proposals and suggestions are welcome. For more information, feel free to contact André Schmer [schmer at ad-tech-group.com].

ATG, May 2017.
