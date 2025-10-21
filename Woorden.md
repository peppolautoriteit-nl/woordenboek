## Algemene termen ##

TBD 

## Peppol BIS termen ##

Concept wordenlijst met beschrijvingen in Nederlands. De volgende termen uit Peppol BIS documenten worden soms verschillend geinterpreteerd. 

| Veld |  Explanation | Uitleg |
|------|--------------|--------|
| cbc:IssueDate   | Invoice issue date  | Factuur uitgiftedatum |
| cbc:DueDate     | Payment due date    | Factuur vervaldatum   | 
| cbc:BuyerReference | Buyer reference  |  Klant referentie     |
| cbc:StartDate   | Invoicing period start date | Begindatum factuurperiode |
| cbc:EndDate     | Invoicing period end date   | Einddatum factuurperiode  |
| cbc:ID          | Purchase order reference    | Inkoopordernummer         |
| cac:Price       | _Aggregate tag to contain the fields below_  |          |
| cbc:PriceAmount | Item net price      |  Netto prijs            |
| cbc:Amount      | Item price discount |  Korting op bruto prijs |
| cbc:BaseAmount  | Item gross price    |  Bruto prijs            |

In sommige gevallen is de aanwezigheid van vergelijkbare velden die tot fouten leidt. Bijvoorbeeld Duedate en Enddate worden door elkaar gehaald. Door een linked data relate te leggen die aangeeft dat het verschillende termen zijn kan dit verduidelijkt worden.
