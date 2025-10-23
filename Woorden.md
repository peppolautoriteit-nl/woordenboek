## Algemene termen

TBD

## Peppol BIS termen

Concept woordenlijst met beschrijvingen in Nederlands. De volgende termen uit
Peppol BIS documenten worden soms verschillend geïnterpreteerd.

**Let op:** De veldnamen zijn nu voorzien van het volledige pad, aangezien
velden zoals `cbc:ID` meerdere keren voorkomen in UBL documenten op
verschillende locaties.

### Document Header Velden

| Volledig Pad             | Explanation (Engels)         | Uitleg (Nederlands)          |
| ------------------------ | ---------------------------- | ---------------------------- |
| cbc:CustomizationID      | Specification identifier     | Specificatie-identificatie   |
| cbc:ProfileID            | Business process type        | Type bedrijfsproces          |
| cbc:ID                   | Invoice number               | Factuurnummer                |
| cbc:IssueDate            | Invoice issue date           | Uitgiftedatum factuur        |
| cbc:DueDate              | Payment due date             | Vervaldatum betaling         |
| cbc:InvoiceTypeCode      | Invoice type code            | Factuurtype code             |
| cbc:Note                 | Invoice note                 | Toelichting op factuur       |
| cbc:TaxPointDate         | Value added tax point date   | BTW-datum                    |
| cbc:DocumentCurrencyCode | Invoice currency code        | Valutacode factuur           |
| cbc:TaxCurrencyCode      | VAT accounting currency code | Valutacode BTW-administratie |

### Factuurperiode

| Volledig Pad                          | Explanation (Engels)            | Uitleg (Nederlands)       |
| ------------------------------------- | ------------------------------- | ------------------------- |
| cac:InvoicePeriod/cbc:StartDate       | Invoicing period start date     | Begindatum factuurperiode |
| cac:InvoicePeriod/cbc:EndDate         | Invoicing period end date       | Einddatum factuurperiode  |
| cac:InvoicePeriod/cbc:DescriptionCode | Value added tax point date code | BTW-datumcode             |

### Document Referenties

| Volledig Pad                                                    | Explanation (Engels)         | Uitleg (Nederlands)              |
| --------------------------------------------------------------- | ---------------------------- | -------------------------------- |
| cac:BillingReference/cac:InvoiceDocumentReference/cbc:ID        | Preceding invoice reference  | Referentie voorgaande factuur    |
| cac:BillingReference/cac:InvoiceDocumentReference/cbc:IssueDate | Preceding invoice issue date | Uitgiftedatum voorgaande factuur |
| cbc:AccountingCost                                              | Buyer accounting reference   | Boekhoudkundige referentie koper |
| cbc:BuyerReference                                              | Buyer reference              | Referentie koper                 |
| cac:OrderReference/cbc:ID                                       | Purchase order reference     | Inkoopordernummer                |
| cac:OrderReference/cbc:SalesOrderID                             | Sales order reference        | Verkoopordernummer               |
| cac:DespatchDocumentReference/cbc:ID                            | Despatch advice reference    | Referentie verzendadvies         |
| cac:ReceiptDocumentReference/cbc:ID                             | Receipt advice reference     | Referentie ontvangstadvies       |
| cac:OriginatorDocumentReference/cbc:ID                          | Tender or lot reference      | Referentie aanbesteding of kavel |
| cac:ContractDocumentReference/cbc:ID                            | Contract reference           | Contractreferentie               |
| cac:ProjectReference/cbc:ID                                     | Project reference            | Projectreferentie                |

### Bijlagen

| Volledig Pad                                                                    | Explanation (Engels)            | Uitleg (Nederlands)                 |
| ------------------------------------------------------------------------------- | ------------------------------- | ----------------------------------- |
| cac:AdditionalDocumentReference/cbc:ID                                          | Supporting document reference   | Referentie ondersteunend document   |
| cac:AdditionalDocumentReference/cbc:DocumentTypeCode                            | Document type code              | Documenttype code                   |
| cac:AdditionalDocumentReference/cbc:DocumentDescription                         | Supporting document description | Beschrijving ondersteunend document |
| cac:AdditionalDocumentReference/cac:Attachment/cbc:EmbeddedDocumentBinaryObject | Attached document               | Bijgevoegd document                 |
| cac:AdditionalDocumentReference/cac:ExternalReference/cbc:URI                   | External document location      | Locatie extern document             |

### Verkoper (Supplier)

| Volledig Pad                                                                               | Explanation (Engels)            | Uitleg (Nederlands)               |
| ------------------------------------------------------------------------------------------ | ------------------------------- | --------------------------------- |
| cac:AccountingSupplierParty/cac:Party/cbc:EndpointID                                       | Electronic address              | Elektronisch adres                |
| cac:AccountingSupplierParty/cac:Party/cac:PartyIdentification/cbc:ID                       | Additional party identification | Aanvullende identificatie partij  |
| cac:AccountingSupplierParty/cac:Party/cac:PartyName/cbc:Name                               | Trading name                    | Handelsnaam                       |
| cac:AccountingSupplierParty/cac:Party/cac:PostalAddress/cbc:StreetName                     | Address line 1                  | Adresregel 1                      |
| cac:AccountingSupplierParty/cac:Party/cac:PostalAddress/cbc:AdditionalStreetName           | Address line 2                  | Adresregel 2                      |
| cac:AccountingSupplierParty/cac:Party/cac:PostalAddress/cbc:CityName                       | City                            | Plaats                            |
| cac:AccountingSupplierParty/cac:Party/cac:PostalAddress/cbc:PostalZone                     | Post code                       | Postcode                          |
| cac:AccountingSupplierParty/cac:Party/cac:PostalAddress/cbc:CountrySubentity               | Country subdivision             | Regio/provincie                   |
| cac:AccountingSupplierParty/cac:Party/cac:PostalAddress/cac:AddressLine/cbc:Line           | Address line 3                  | Adresregel 3                      |
| cac:AccountingSupplierParty/cac:Party/cac:PostalAddress/cac:Country/cbc:IdentificationCode | Country                         | Land                              |
| cac:AccountingSupplierParty/cac:Party/cac:PartyTaxScheme/cbc:CompanyID                     | VAT identifier                  | BTW-identificatienummer           |
| cac:AccountingSupplierParty/cac:Party/cac:PartyLegalEntity/cbc:RegistrationName            | Formal name of the seller       | Officiële naam verkoper           |
| cac:AccountingSupplierParty/cac:Party/cac:PartyLegalEntity/cbc:CompanyID                   | Legal registration identifier   | KvK-nummer                        |
| cac:AccountingSupplierParty/cac:Party/cac:PartyLegalEntity/cbc:CompanyLegalForm            | Additional legal information    | Aanvullende juridische informatie |
| cac:AccountingSupplierParty/cac:Party/cac:Contact/cbc:Name                                 | Contact point                   | Naam contactpersoon               |
| cac:AccountingSupplierParty/cac:Party/cac:Contact/cbc:Telephone                            | Contact telephone number        | Telefoonnummer contactpersoon     |
| cac:AccountingSupplierParty/cac:Party/cac:Contact/cbc:ElectronicMail                       | Contact email address           | E-mailadres contactpersoon        |

### Koper (Customer)

| Volledig Pad                                                                               | Explanation (Engels)            | Uitleg (Nederlands)              |
| ------------------------------------------------------------------------------------------ | ------------------------------- | -------------------------------- |
| cac:AccountingCustomerParty/cac:Party/cbc:EndpointID                                       | Electronic address              | Elektronisch adres               |
| cac:AccountingCustomerParty/cac:Party/cac:PartyIdentification/cbc:ID                       | Additional party identification | Aanvullende identificatie partij |
| cac:AccountingCustomerParty/cac:Party/cac:PartyName/cbc:Name                               | Trading name                    | Handelsnaam                      |
| cac:AccountingCustomerParty/cac:Party/cac:PostalAddress/cbc:StreetName                     | Address line 1                  | Adresregel 1                     |
| cac:AccountingCustomerParty/cac:Party/cac:PostalAddress/cbc:AdditionalStreetName           | Address line 2                  | Adresregel 2                     |
| cac:AccountingCustomerParty/cac:Party/cac:PostalAddress/cbc:CityName                       | City                            | Plaats                           |
| cac:AccountingCustomerParty/cac:Party/cac:PostalAddress/cbc:PostalZone                     | Post code                       | Postcode                         |
| cac:AccountingCustomerParty/cac:Party/cac:PostalAddress/cbc:CountrySubentity               | Country subdivision             | Regio/provincie                  |
| cac:AccountingCustomerParty/cac:Party/cac:PostalAddress/cac:AddressLine/cbc:Line           | Address line 3                  | Adresregel 3                     |
| cac:AccountingCustomerParty/cac:Party/cac:PostalAddress/cac:Country/cbc:IdentificationCode | Country                         | Land                             |
| cac:AccountingCustomerParty/cac:Party/cac:PartyTaxScheme/cbc:CompanyID                     | VAT identifier                  | BTW-identificatienummer          |
| cac:AccountingCustomerParty/cac:Party/cac:PartyLegalEntity/cbc:RegistrationName            | Formal name of the buyer        | Officiële naam koper             |
| cac:AccountingCustomerParty/cac:Party/cac:PartyLegalEntity/cbc:CompanyID                   | Legal registration identifier   | KvK-nummer                       |
| cac:AccountingCustomerParty/cac:Party/cac:Contact/cbc:Name                                 | Contact point                   | Naam contactpersoon              |
| cac:AccountingCustomerParty/cac:Party/cac:Contact/cbc:Telephone                            | Contact telephone number        | Telefoonnummer contactpersoon    |
| cac:AccountingCustomerParty/cac:Party/cac:Contact/cbc:ElectronicMail                       | Contact email address           | E-mailadres contactpersoon       |

### Begunstigde en Fiscaal Vertegenwoordiger

| Volledig Pad                                                                    | Explanation (Engels)              | Uitleg (Nederlands)                  |
| ------------------------------------------------------------------------------- | --------------------------------- | ------------------------------------ |
| cac:PayeeParty/cac:PartyName/cbc:Name                                           | Payee name                        | Naam begunstigde                     |
| cac:PayeeParty/cac:PartyLegalEntity/cbc:CompanyID                               | Legal registration identifier     | KvK-nummer                           |
| cac:TaxRepresentativeParty/cac:PartyName/cbc:Name                               | Tax representative name           | Naam fiscaal vertegenwoordiger       |
| cac:TaxRepresentativeParty/cac:PostalAddress/cac:Country/cbc:IdentificationCode | Tax representative country        | Land fiscaal vertegenwoordiger       |
| cac:TaxRepresentativeParty/cac:PartyTaxScheme/cbc:CompanyID                     | Tax representative VAT identifier | BTW-nummer fiscaal vertegenwoordiger |

### Levering

| Volledig Pad                                                                     | Explanation (Engels) | Uitleg (Nederlands)       |
| -------------------------------------------------------------------------------- | -------------------- | ------------------------- |
| cac:Delivery/cbc:ActualDeliveryDate                                              | Actual delivery date | Werkelijke leveringsdatum |
| cac:Delivery/cac:DeliveryLocation/cbc:ID                                         | Location identifier  | Locatie-identificatie     |
| cac:Delivery/cac:DeliveryLocation/cac:Address/cbc:StreetName                     | Address line 1       | Adresregel 1              |
| cac:Delivery/cac:DeliveryLocation/cac:Address/cbc:CityName                       | City                 | Plaats                    |
| cac:Delivery/cac:DeliveryLocation/cac:Address/cbc:PostalZone                     | Post code            | Postcode                  |
| cac:Delivery/cac:DeliveryLocation/cac:Address/cac:Country/cbc:IdentificationCode | Deliver to country   | Land afleveradres         |
| cac:Delivery/cac:DeliveryParty/cac:PartyName/cbc:Name                            | Delivery party name  | Naam afleverpartij        |

### Betaling

| Volledig Pad                                                                     | Explanation (Engels)                | Uitleg (Nederlands)          |
| -------------------------------------------------------------------------------- | ----------------------------------- | ---------------------------- |
| cac:PaymentMeans/cbc:PaymentMeansCode                                            | Payment means type code             | Code betaalwijze             |
| cac:PaymentMeans/cbc:PaymentID                                                   | Remittance information              | Betalingskenmerk             |
| cac:PaymentMeans/cac:CardAccount/cbc:PrimaryAccountNumberID                      | Payment card primary account number | Betaalkaartnummer            |
| cac:PaymentMeans/cac:CardAccount/cbc:NetworkID                                   | Card network identifier             | Identificatie kaartnetwerk   |
| cac:PaymentMeans/cac:CardAccount/cbc:HolderName                                  | Payment card holder name            | Naam kaarthouder             |
| cac:PaymentMeans/cac:PayeeFinancialAccount/cbc:ID                                | Payment account identifier          | Rekeningnummer (IBAN)        |
| cac:PaymentMeans/cac:PayeeFinancialAccount/cbc:Name                              | Payment account name                | Naam rekeninghouder          |
| cac:PaymentMeans/cac:PayeeFinancialAccount/cac:FinancialInstitutionBranch/cbc:ID | Payment service provider identifier | BIC-code                     |
| cac:PaymentMeans/cac:PaymentMandate/cbc:ID                                       | Mandate reference identifier        | Incassomachtigingskenmerk    |
| cac:PaymentMeans/cac:PaymentMandate/cac:PayerFinancialAccount/cbc:ID             | Debited account identifier          | Nummer gedebiteerde rekening |
| cac:PaymentTerms/cbc:Note                                                        | Payment terms                       | Betalingsvoorwaarden         |

### Document Kortingen en Toeslagen

| Volledig Pad                                      | Explanation (Engels)              | Uitleg (Nederlands)            |
| ------------------------------------------------- | --------------------------------- | ------------------------------ |
| cac:AllowanceCharge/cbc:ChargeIndicator           | Indicator for allowance or charge | Indicator korting of toeslag   |
| cac:AllowanceCharge/cbc:AllowanceChargeReasonCode | Allowance or charge reason code   | Code reden korting of toeslag  |
| cac:AllowanceCharge/cbc:AllowanceChargeReason     | Allowance or charge reason        | Reden korting of toeslag       |
| cac:AllowanceCharge/cbc:MultiplierFactorNumeric   | Allowance or charge percentage    | Percentage korting of toeslag  |
| cac:AllowanceCharge/cbc:Amount                    | Allowance or charge amount        | Bedrag korting of toeslag      |
| cac:AllowanceCharge/cbc:BaseAmount                | Allowance or charge base amount   | Basisbedrag korting of toeslag |
| cac:AllowanceCharge/cac:TaxCategory/cbc:ID        | VAT category code                 | BTW-categoriecode              |
| cac:AllowanceCharge/cac:TaxCategory/cbc:Percent   | VAT rate                          | BTW-tarief                     |

### BTW Totalen

| Volledig Pad                                                            | Explanation (Engels)        | Uitleg (Nederlands)         |
| ----------------------------------------------------------------------- | --------------------------- | --------------------------- |
| cac:TaxTotal/cbc:TaxAmount                                              | Invoice total VAT amount    | Totaal BTW-bedrag factuur   |
| cac:TaxTotal/cac:TaxSubtotal/cbc:TaxableAmount                          | VAT category taxable amount | Belastbaar bedrag           |
| cac:TaxTotal/cac:TaxSubtotal/cbc:TaxAmount                              | VAT category tax amount     | BTW-bedrag                  |
| cac:TaxTotal/cac:TaxSubtotal/cac:TaxCategory/cbc:ID                     | VAT category code           | BTW-categoriecode           |
| cac:TaxTotal/cac:TaxSubtotal/cac:TaxCategory/cbc:Percent                | VAT category rate           | BTW-tarief                  |
| cac:TaxTotal/cac:TaxSubtotal/cac:TaxCategory/cbc:TaxExemptionReasonCode | VAT exemption reason code   | Code BTW-vrijstellingsreden |
| cac:TaxTotal/cac:TaxSubtotal/cac:TaxCategory/cbc:TaxExemptionReason     | VAT exemption reason        | Reden BTW-vrijstelling      |

### Document Totalen

| Volledig Pad                                     | Explanation (Engels)                | Uitleg (Nederlands)         |
| ------------------------------------------------ | ----------------------------------- | --------------------------- |
| cac:LegalMonetaryTotal/cbc:LineExtensionAmount   | Sum of Invoice line net amount      | Som netto regelbedragen     |
| cac:LegalMonetaryTotal/cbc:TaxExclusiveAmount    | Invoice total amount without VAT    | Factuurtotaal exclusief BTW |
| cac:LegalMonetaryTotal/cbc:TaxInclusiveAmount    | Invoice total amount with VAT       | Factuurtotaal inclusief BTW |
| cac:LegalMonetaryTotal/cbc:AllowanceTotalAmount  | Sum of allowances on document level | Totaal kortingen            |
| cac:LegalMonetaryTotal/cbc:ChargeTotalAmount     | Sum of charges on document level    | Totaal toeslagen            |
| cac:LegalMonetaryTotal/cbc:PrepaidAmount         | Paid amount                         | Vooruitbetaald bedrag       |
| cac:LegalMonetaryTotal/cbc:PayableRoundingAmount | Rounding amount                     | Afrondingsbedrag            |
| cac:LegalMonetaryTotal/cbc:PayableAmount         | Amount due for payment              | Te betalen bedrag           |

### Factuurregels

| Volledig Pad                                               | Explanation (Engels)                    | Uitleg (Nederlands)               |
| ---------------------------------------------------------- | --------------------------------------- | --------------------------------- |
| cac:InvoiceLine/cbc:ID                                     | Invoice line identifier                 | Regelnummer                       |
| cac:InvoiceLine/cbc:Note                                   | Invoice line note                       | Toelichting op regel              |
| cac:InvoiceLine/cbc:InvoicedQuantity                       | Invoiced quantity                       | Gefactureerde hoeveelheid         |
| cac:InvoiceLine/cbc:InvoicedQuantity/@unitCode             | Unit of measure code                    | Code maateenheid                  |
| cac:InvoiceLine/cbc:LineExtensionAmount                    | Invoice line net amount                 | Netto regelbedrag                 |
| cac:InvoiceLine/cbc:AccountingCost                         | Invoice line Buyer accounting reference | Boekhoudkundige referentie koper  |
| cac:InvoiceLine/cac:InvoicePeriod/cbc:StartDate            | Invoice line period start date          | Begindatum regelperiode           |
| cac:InvoiceLine/cac:InvoicePeriod/cbc:EndDate              | Invoice line period end date            | Einddatum regelperiode            |
| cac:InvoiceLine/cac:OrderLineReference/cbc:LineID          | Referenced purchase order line          | Referentie inkooporderregel       |
| cac:InvoiceLine/cac:DocumentReference/cbc:ID               | Invoice line object identifier          | Object-identificatie factuurregel |
| cac:InvoiceLine/cac:DocumentReference/cbc:DocumentTypeCode | Document type code                      | Documenttype code                 |

### Factuurregels - Kortingen en Toeslagen

| Volledig Pad                                                      | Explanation (Engels)                       | Uitleg (Nederlands)                     |
| ----------------------------------------------------------------- | ------------------------------------------ | --------------------------------------- |
| cac:InvoiceLine/cac:AllowanceCharge/cbc:ChargeIndicator           | Indicator for allowance or charge          | Indicator korting of toeslag            |
| cac:InvoiceLine/cac:AllowanceCharge/cbc:AllowanceChargeReasonCode | Line level allowance or charge reason code | Code reden korting of toeslag op regel  |
| cac:InvoiceLine/cac:AllowanceCharge/cbc:AllowanceChargeReason     | Line level allowance or charge reason      | Reden korting of toeslag op regel       |
| cac:InvoiceLine/cac:AllowanceCharge/cbc:MultiplierFactorNumeric   | Line level allowance or charge percentage  | Percentage korting of toeslag op regel  |
| cac:InvoiceLine/cac:AllowanceCharge/cbc:Amount                    | Line level allowance or charge amount      | Bedrag korting of toeslag op regel      |
| cac:InvoiceLine/cac:AllowanceCharge/cbc:BaseAmount                | Line level allowance or charge base amount | Basisbedrag korting of toeslag op regel |

### Factuurregels - Artikelinformatie

| Volledig Pad                                                                    | Explanation (Engels)            | Uitleg (Nederlands)                  |
| ------------------------------------------------------------------------------- | ------------------------------- | ------------------------------------ |
| cac:InvoiceLine/cac:Item/cbc:Description                                        | Item description                | Artikelbeschrijving                  |
| cac:InvoiceLine/cac:Item/cbc:Name                                               | Item name                       | Artikelnaam                          |
| cac:InvoiceLine/cac:Item/cac:BuyersItemIdentification/cbc:ID                    | Item Buyer's identifier         | Artikelnummer koper                  |
| cac:InvoiceLine/cac:Item/cac:SellersItemIdentification/cbc:ID                   | Item Seller's identifier        | Artikelnummer verkoper               |
| cac:InvoiceLine/cac:Item/cac:StandardItemIdentification/cbc:ID                  | Item standard identifier        | Standaard artikelnummer (bijv. GTIN) |
| cac:InvoiceLine/cac:Item/cac:OriginCountry/cbc:IdentificationCode               | Item country of origin          | Land van herkomst artikel            |
| cac:InvoiceLine/cac:Item/cac:CommodityClassification/cbc:ItemClassificationCode | Item classification identifier  | Artikelclassificatie                 |
| cac:InvoiceLine/cac:Item/cac:ClassifiedTaxCategory/cbc:ID                       | Invoiced item VAT category code | BTW-categoriecode artikel            |
| cac:InvoiceLine/cac:Item/cac:ClassifiedTaxCategory/cbc:Percent                  | Invoiced item VAT rate          | BTW-tarief artikel                   |
| cac:InvoiceLine/cac:Item/cac:AdditionalItemProperty/cbc:Name                    | Item attribute name             | Naam artikelkenmerk                  |
| cac:InvoiceLine/cac:Item/cac:AdditionalItemProperty/cbc:Value                   | Item attribute value            | Waarde artikelkenmerk                |

### Factuurregels - Prijsinformatie

| Volledig Pad                                                 | Explanation (Engels)     | Uitleg (Nederlands)     |
| ------------------------------------------------------------ | ------------------------ | ----------------------- |
| cac:InvoiceLine/cac:Price/cbc:PriceAmount                    | Item net price           | Netto artikelprijs      |
| cac:InvoiceLine/cac:Price/cbc:BaseQuantity                   | Item price base quantity | Basishoeveelheid prijs  |
| cac:InvoiceLine/cac:Price/cac:AllowanceCharge/cbc:Amount     | Item price discount      | Korting op artikelprijs |
| cac:InvoiceLine/cac:Price/cac:AllowanceCharge/cbc:BaseAmount | Item gross price         | Bruto artikelprijs      |

## Veelvoorkomende verwarring

In sommige gevallen is de aanwezigheid van vergelijkbare velden die tot fouten
leidt. Door het volledige pad aan te geven wordt deze verwarring verminderd:

- **cbc:DueDate** (vervaldatum betaling op documentniveau) vs
  **cac:InvoicePeriod/cbc:EndDate** (einddatum factuurperiode)
- **cbc:ID** komt op vele plaatsen voor:
  - Documentniveau: factuurnummer
  - In cac:OrderReference: inkoopordernummer
  - In cac:InvoiceLine: regelnummer
  - In cac:AdditionalDocumentReference: documentreferentie
- **cac:InvoiceLine/cac:Price/cbc:PriceAmount** (netto artikelprijs) vs
  **cac:InvoiceLine/cac:Price/cac:AllowanceCharge/cbc:BaseAmount** (bruto
  artikelprijs)

Door een linked data relatie te leggen die het volledige pad aangeeft, kan dit
verduidelijkt worden.
