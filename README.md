# Swap Rate Curve

Market observable interest rate curves are mainly swap curves and bond curves. They consist of market observable quotations, such as bond prices, swap rates, basis swap spreads, interest rate futures prices, or deposit rates. Bond curves are the term structure of market quoted bond prices, while swap curves are the term structures of swap rates, basis swap spreads, or Eurodollar futures. Swap curves can be futher divided into base swap curves and basis swap curves. Normally the 3 month swap curve is the base curve as all the basis curves are quoted against it. The market observable curves cannot be used for valuation directly. Thus they need to be bootstrapped into the derived curves that are essential for asset pricing.

Swap curves can be categoried into swap rate curves, basis curves, and OIS curves. Usully a swap rate curve is also called a base curve or standard curve or 3 month swap curve. The reason for calling 3 month curve as base curve is all the other (basis) curves are quoted against it.

The swap rate curve consists of a set of the most liquid and dominant interest rate products for certain time horizons. Normally the curve is divided into three parts. The short end of the term structure is determined by deposit rates. The middle part of the curve uses Eurodollar futures or FRAs. The far end is given by mid swap rates.

Swap rate curve is the base element for constructing all yield curves. It consists of a set of the most liquid and dominant interest rate instruments in selected time horizons. Normally the curve is divided into three parts. The short end of the term structure is determined by deposit rates. The middle part of the curve uses Eurodollar futures or FRA. The far end is given by mid swap rates.

FinPricing does data collecttion, pre-process, and reconciliation for you. The curves delivered are ready to use. These curves are actually used by our analytic engine. We guaratee they can be successfully bootstrapped and calibrated. A swap rate curve sample data is shown below:

Date	CurveName	QuoteName	Instrument	Value
11/17/2020	USD_3M	DepositRate.USD.LIBOR.3M	Cash      	0.00231
11/17/2020	USD_3M	Future.USD.ED 3M.MAR21	FUTURE    	99.785
11/17/2020	USD_3M	Future.USD.ED 3M.JUN21	FUTURE    	99.79
11/17/2020	USD_3M	Future.USD.ED 3M.SEP21	FUTURE    	99.785
11/17/2020	USD_3M	Future.USD.ED 3M.DEC21	FUTURE    	99.75
11/17/2020	USD_3M	Future.USD.ED 3M.MAR22	FUTURE    	99.69
11/17/2020	USD_3M	Future.USD.ED 3M.JUN22	FUTURE    	99.68
11/17/2020	USD_3M	Future.USD.ED 3M.SEP22	FUTURE    	99.665

You can find more details at
https://finpricing.com/lib/IrCurveIntroduction.html
