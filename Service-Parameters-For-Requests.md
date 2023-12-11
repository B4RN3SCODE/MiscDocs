Here is a that outlines *most* of the complicated items I will have to query and processes.  Initial thoughts/considerations:

- Most of the large requests have data that will be passed to me via API. So that data will be easier to fill
- I still need default values for some of the fields that will not be included in the request to me
- A lot of the request have the same property or parameter name, we only have to solve it once, obviously
- The `RequestID` fields listed is a variable I will generate to track the communication between my app and the web service, can ignore this
- The other system/server/metadata fields I need values for

# Service: ivpwsEO001

To save time, I will only include the major endpoints.

*If you know good default values or the system/server/metadata properties, or you know good default values for the less common properties that may not be passed to my API, please copy/paste the list and send me anything you come up with*

### Legend:

- "..." means that it's probably coming from the API input (feel free to note if I am wrong)
- "???" means I am not sure what how to handle/populate the field
- "(Some note text)" are my thoughts regarding it, open to ideas
- An checked item means its solved... i think


**Keep in mind** some of these may be solved/easier to solve when i have successful requests.  I am guessing on a few of the fields.  If you can find documentation before Epocor responds, reach out any time.


## AddCreditCardAuthorizationDetail

- [x] `RequestID`              (Field I use to track the communication between web app and their web service)
- [ ] `RequestMode`            ???
- [x] `CMSDataBase`            (The database name i.e. TST7)
- [x] `ServLang`              (ENU, found on config page)
- [ ] `ServPlntCod`            ???
- [ ] `CustomizedLibrary`      ( CMSCUSCIA ??? )
- [ ] `DocumentType`           ???
- [ ] `DocumentNumber`         ??? (guessing just a unique ID to track this communication)
- [ ] `DocumentReleaseNumber`  ???
- [x] `TransactionToken`       ...
- [x] `CreditCardLast4Digits`  ...
- [ ] `TransactionReference`   ( come from API ??? )
- [ ] `ARCode`                 ???
- [x] `AuthorizeByUser`        ...
- [x] `AuthorizeAmount`        ...
- [x] `AuthorizationNumber`    ...
- [x] `AuthorizeDate`          ...
- [x] `AuthorizeTime`          ...
- [ ] `AuthorizeExpireDate`    ???
- [ ] `AuthorizeStatus`        ...???
- [ ] `SettleByUser`           ???
- [ ] `SettleAmount`           ???
- [ ] `SettleDate`             ???
- [ ] `SettleTime`             ???
- [ ] `SettleStatus`           ???
- [ ] `SettleBatchNumber`      ???
- [ ] `VoidByUser`             ???
- [ ] `VoidAmount`             ???
- [ ] `VoidDate`               ???
- [ ] `VoidTime`               ???
- [ ] `RefundByUser`           ???
- [ ] `RefundAmount`           ???
- [ ] `RefundDate`             ???
- [ ] `RefundTime`             ???
- [ ] `RefundStatus`           ???
- [ ] `RefundRefNumber`        ???


## AddCreditCardAuthorizationHeader

- [x] `RequestID`               (Field I use to track the communication between web app and their web service)
- [ ] `RequestMode`             ???
- [x] `CMSDataBase`             (The database name i.e. TST7)
- [x] `ServLang`                (ENU, found on config page)
- [ ] `ServPlntCod`             ???
- [ ] `CustomizedLibrary`       ( CMSCUSCIA ??? )
- [ ] `DocumentType`            ???
- [ ] `DocumentNumber`          ??? (guessing just a unique ID to track this communication)
- [ ] `DocumentReleaseNumber`   ???
- [ ] `CustomerType`            ???
- [ ] `CustomerNumber`          ...
- [ ] `CreditCardCode`          ...???
- [ ] `ARCode`                  ???
- [ ] `CreditCardLast4Digits`   ...
- [ ] `CardHolder`              ...
- [ ] `PlantCode`               ...???
- [ ] `ProcessByInterface`      ???
- [ ] `ProcessByNetwork`        ???
- [ ] `MerchantCode`            ...???
- [ ] `Currency`                ...
- [ ] `Status`                  ...
- [x] `AuthorizeByUser`        ...
- [x] `AuthorizeAmount`        ...
- [x] `AuthorizationNumber`    ...
- [x] `AuthorizeDate`          ...
- [x] `AuthorizeTime`          ...
- [ ] `AuthorizeExpireDate`    ???
- [ ] `SettleByUser`
- [ ] `SettleAmount`
- [ ] `SettleDate`
- [ ] `SettleTime`
- [ ] `SettleBatchNumber`
- [ ] `VoidByUser`
- [ ] `VoidAmount`
- [ ] `VoidDate`
- [ ] `VoidTime`
- [ ] `RefundByUser`
- [ ] `RefundAmount`
- [ ] `RefundDate`
- [ ] `RefundTime`
- [ ] `RefundRefNumber`
- [ ] `TransactionReference`
- [ ] `TransactionToken`
- [ ] `CreditCardArchiveKey`
- [ ] `SalesOrder`
- [ ] `AttachToBOL`
- [ ] `AttachToInvoice`
- [ ] `InvoiceCreditFlag`
- [ ] `InvoiceStatus`
- [ ] `OrderAmount`
- [ ] `BOLAmount`
- [ ] `InvoiceAmount`
- [ ] `FreightAmount`
- [ ] `FreightTax`


## InquireCreditCardAuthorizationDetail

- [x] `RequestID`
- [ ] `RequestMode`         ???
- [x] `CMSDataBase`
- [x] `ServLang`
- [ ] `ServPlntCod`         ???
- [ ] `CustomizedLibrary`   ??? see above
- [ ] `DocumentType`        ???
- [ ] `DocumentNumber`      ???
- [ ] `TransactionToken`    ...


## InquireCreditCardAuthorizationHeader

- [ ] `RequestID`
- [ ] `RequestMode`
- [ ] `CMSDataBase`
- [ ] `ServLang`
- [ ] `ServPlntCod`
- [ ] `CustomizedLibrary`
- [ ] `DocumentType`
- [ ] `DocumentNumber`


## AddSalesOrderHeaderType

- [ ] `RequestID`
- [ ] `RequestMode`
- [ ] `CMSDataBase`
- [ ] `ServLang`
- [ ] `ServPlntCod`
- [ ] `CustomizedLibrary`
- [ ] `OrderNumber`
- [ ] `Quote`
- [ ] `Credit`
- [ ] `DateEntered`
- [ ] `OrderType`
- [ ] `BilltoCustomer`
- [ ] `Attention`
- [ ] `PhoneNumber`
- [ ] `ShiptoCustomer`
- [ ] `ShipToType`
- [ ] `ShipToConsumer`
- [ ] `CustomerClientNbr`
- [ ] `ShiptoName`
- [ ] `ShiptoAddress1` to `ShiptoAddress10`
- [ ] `ShiptoPostalCode`
- [ ] `ShiptoCity`
- [ ] `ShiptoProvinceCode`
- [ ] `ShiptoCountryCode`
- [ ] `TermsCode`
- [ ] `PayByCreditcard`
- [ ] `CustomerPurchaseOrder`
- [ ] `RefertoQuoteNumber`
- [ ] `CustomerReference`
- [ ] `ShipVia`
- [ ] `RequiredDate`
- [ ] `RequiredTime`
- [ ] `CancelDate`
- [ ] `DefaultStockLoc`
- [ ] `ShipComplete`
- [ ] `AllowBackorder`
- [ ] `ReferenceInvoice`
- [ ] `SalesAgent`
- [ ] `CommissionPercentage`
- [ ] `CommissionRate`
- [ ] `FOBCode`
- [ ] `PrepaidCollectInvoice`
- [ ] `CarrierCode`
- [ ] `ServiceCode`
- [ ] `GSTLicence`
- [ ] `PSTLicence`
- [ ] `DepartmentNumber`
- [ ] `PromotionNumber`
- [ ] `ExpeditedOrder`
- [ ] `PlantCode`
- [ ] `SaturdayDelivery`
- [ ] `SaturdayPickup`
- [ ] `SalesChannelCode`
- [ ] `AutoReleaseBillByOrderInvoice`
- [ ] `BillByOrder`
- [ ] `PostBillByOrderInvoice`
- [ ] `Permit4473`
- [ ] `ExemptExportPermitNumber`
- [ ] `StateCountyFOID`
- [ ] `ExternalOrderNbr`
- [ ] `UpdateOrderApplyWholeOrderDiscount`
- [ ] `UpdateOrderApplyGLSalesToItem`
- [ ] `UpdateOrderApplyCommissionRateAndPercentage`
- [ ] `UpdateOrderApplyTaxGroupRateToItem`
- [ ] `UpdateOrderChangePlant`
- [ ] `NotepadTexts` (array of `NotepadTextType`)
- [ ] `UserDefinedFields` (array of `UserDefinedFieldType`)
- [ ] `CommissionSplits` (array of `CommissionSplitType`)
- [ ] `EmptyField01` to `EmptyField80`
- [ ] `OrderRevisionReason`
- [ ] `PricePackages` (array of `PricePackageType`)
- [ ] `PrintSendOrderAcknowledgement`
- [ ] `PrintSendOption`
- [ ] `SendByFaxOrEmail`
- [ ] `SendToCustomerBillToShipToAddress`
- [ ] `FaxDate`
- [ ] `FaxTime`
- [ ] `FaxToContactName`
- [ ] `FaxNumber`
- [ ] `RecipientEmailAddress`
- [ ] `SenderEmailAddress`
- [ ] `EmailSubject`
- [ ] `EmailMessageBody`
- [ ] `EmailSendType`


## AddSalesOrderItemType

- [ ] `RequestID`
- [ ] `RequestMode`
- [ ] `CMSDataBase`
- [ ] `ServLang`
- [ ] `ServPlntCod`
- [ ] `CustomizedLibrary`
- [ ] `OrderNumber`
- [ ] `ItemNumber`
- [ ] `Quote`
- [ ] `Credit`
- [ ] `ReturnAuthDocNbr`
- [ ] `ReturnAuthDocItemNbr`
- [ ] `AllowLateShipment`
- [ ] `DirectBuy`
- [ ] `DirectBuyAction`
- [ ] `SCDPart`
- [ ] `PartNumber`
- [ ] `QuantityOrdered`
- [ ] `OrderUnit`
- [ ] `ProjectNumber`
- [ ] `CustomerRANNumber`
- [ ] `UnitPrice`
- [ ] `PricingUnit`
- [ ] `SalesAgent`
- [ ] `CustomerPOItemNbr`
- [ ] `CommissionPercentage`
- [ ] `CommissionRate`
- [ ] `GLDistributionCode`
- [ ] `CreditReasonCode`
- [ ] `TaxGroupCode`
- [ ] `TaxRatecode`
- [ ] `MajorSalesCode`
- [ ] `MinorSalesCode`
- [ ] `PromiseDate`
- [ ] `PromiseTime`
- [ ] `StockLocation`
- [ ] `CancelDate`
- [ ] `RequestDate`
- [ ] `RequestTime`
- [ ] `LoadSequenceNumber`
- [ ] `DoNotShipBeforeDate`
- [ ] `FreightAmount`
- [ ] `PickType`
- [ ] `PriceLock`
- [ ] `CustomerRevisionNumber`
- [ ] `CustomerAliasPartNumber`
- [ ] `PerUnitFreightInOrderUnit`
- [ ] `HandlingFeePercentage`
- [ ] `ConsignmentPart`
- [ ] `AvailableToShipPickGroup`
- [ ] `FreightDetailCarrierCode`
- [ ] `FreightDetailServiceCode`
- [ ] `FreightDetailStandardFreightPerWeightUnit`
- [ ] `FreightDetailWeightUnit`
- [ ] `FreightDetailSurchargePercentage`
- [ ] `FreightDetailPerSkidSpotAmount`
- [ ] `FreightDetailFlatFreight`
- [ ] `FeatureAndOptionModelCode`
- [ ] `ServiceAgreementNumber`
- [ ] `RegisteredProductNbr`
- [ ] `CreateWorkOrderFromFeatureAndOptions`
- [ ] `FeatureAndOptionDetails` (array of `FeatureAndOptionDetailType`)
- [ ] `ItemDescriptions` (array of `ItemDescriptionType`)
- [ ] `NotepadTexts` (array of `NotepadTextType`)
- [ ] `UserDefinedFields` (array of `UserDefinedFieldType`)
- [ ] `ComplementaryItems` (array of `ComplementaryItemType`)
- [ ] `ATSSubDetails` (array of `ATSSubDetailType`)
- [ ] `CommissionSplits` (array of `CommissionSplitType`)
- [ ] `EmptyField01` to `EmptyField80`



