# Caleb's Modernized E-Movies

This is my modernized version of the emovies.erwin data model. Below is a list of changes and additions I made.

TWO overarching changes:
    Adding streaming and ERental capabilities
    Adding new E-pay options

Entity changes:
    -MovieRentalRecord (is now a parent type with EBuy and PhysicalRental as children)
    -Payment (is now a parent type with three children: BitcoinPayment, PaypalPayment, CreditCardPayment)


Entity additions:
    1) PhysicalMovie
    2) EBuy
    3) DigitalRental
    4) StreamMovie
    5) BitcoinPayment
    6) PaypalPayment
    7) CreditCardPayment

*Paypal and Bitcoin transactions will likely take place on third-party platforms, but we store basic information in the DB
    -potential security concerns with this?

    

