# Multi-currency support

@@name supports reporting of all value transactions in both their original currency and also the base currency for the enterprise company.

This allows easy consolidation of all transaction values in the base currency, while preserving the original values.

## How it works

All value transactions in @@name are recorded in (at least) two currencies in parallel - in the original and the base.

The original currency records the transaction value as it is.
The value is then converted to the base currency.

The rule for conversion depend on the nature of the value, but is usually conversion, according to an attached currency rates directory.
The conversion can also be performed based on average valuation of an account in original vs base currency.
Other methods might also apply.
