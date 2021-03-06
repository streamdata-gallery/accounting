---
swagger: "2.0"
x-collection-name: Intuit
x-complete: 0
info:
  title: QuickBooks Online V3 API Get Purchase Order
  description: |-
    Read a puchase-order object
    Method : POST
  version: 1.0.0
host: DefaultParameterValue
basePath: /v3/company/DefaultParameterValue
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cdc:
    get:
      summary: Get CDC
      description: |-
        Retrive changed Bill and invoice objects since Aug10,2016
        Method - GET
      operationId: getCdc
      x-api-path-slug: cdc-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: changedSince
      - in: header
        name: Content-Type
      - in: query
        name: entities
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - CDC
  /query:
    post:
      summary: Post Query
      description: |-
        Read all transfer objects using the 'Query' endpoint
        Method : POST
      operationId: postQuery
      x-api-path-slug: query-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Query
  /estimate/163:
    get:
      summary: Get Estimate
      description: |-
        Read an Estimate object by Id
        Method : POST
      operationId: getEstimate163
      x-api-path-slug: estimate163-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Estimate
  /invoice:
    post:
      summary: Post Invoice
      description: |-
        Create an invoice object
        Method : POST
      operationId: postInvoice
      x-api-path-slug: invoice-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Invoice
  /term:
    post:
      summary: Post Term
      description: |-
        Update a term object
        Method : POST

        Term object can't be deleted parmanently. It can only be deactived by setting the 'Active' attribute to false.
      operationId: postTerm
      x-api-path-slug: term-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Term
  /preferences:
    get:
      summary: Get Preferences
      description: |-
        Read the preference object
        Method : POST
      operationId: getPreferences
      x-api-path-slug: preferences-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Preferences
    post:
      summary: Post Preferences
      description: |-
        Update the preference object endpoint
        Method : POST
      operationId: postPreferences
      x-api-path-slug: preferences-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Preferences
  /reports/InventoryValuationSummary:
    get:
      summary: Get Reports Inventory Valuation Summary
      description: |-
        Report - Inventory Valuation Summary
        Method : GET

        Docs - https://developer.intuit.com/docs/api/accounting/inventory%20valuation
      operationId: getReportsInventoryvaluationsummary
      x-api-path-slug: reportsinventoryvaluationsummary-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Inventory
      - Valuation
      - Summary
  /purchase:
    post:
      summary: Post Purchase
      description: |-
        Create a puchase object
        Method : POST
      operationId: postPurchase
      x-api-path-slug: purchase-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Purchase
  /salesreceipt/181:
    get:
      summary: Get SaleS Receipt
      description: |-
        Create an salesreceipt object
        Method : POST
      operationId: getSalesreceipt181
      x-api-path-slug: salesreceipt181-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - SaleS
      - Receipt
  /deposit:
    post:
      summary: Post Deposit
      description: |-
        Update a deposit object
        Method : POST
      operationId: postDeposit
      x-api-path-slug: deposit-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Deposit
  /transfer:
    post:
      summary: Post Transfer
      description: |-
        Create a transfer object
        Method : POST
      operationId: postTransfer
      x-api-path-slug: transfer-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Transfer
  /bill:
    post:
      summary: Post Bill
      description: |-
        Create a bill
        Content-Type:application/json
        Method - POST
      operationId: postBill
      x-api-path-slug: bill-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Bill
  /account/1:
    get:
      summary: Get Account
      description: Get the Account which has accountId as 1
      operationId: getAccount1
      x-api-path-slug: account1-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Account
  /invoice/147:
    get:
      summary: Get Invoice
      description: |-
        Read an invoice object by Id
        Method : POST
      operationId: getInvoice147
      x-api-path-slug: invoice147-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Invoice
  /reports/CustomerBalanceDetail:
    get:
      summary: Get Reports Customer Balance Detail
      description: |-
        Report - CustomerBalance Detail
        Method : GET

        The information below provides a reference on how to access the Customer Balance Detail report from the QuickBooks Online Report Service.
      operationId: getReportsCustomerbalancedetail
      x-api-path-slug: reportscustomerbalancedetail-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Customer
      - Balance
      - Detail
  /payment:
    post:
      summary: Post Payment
      description: |-
        Create an payment object
        Method : POST
      operationId: postPayment
      x-api-path-slug: payment-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Payment
  /reports/ProfitAndLossDetail:
    get:
      summary: Get Reports Profit and Loss DETAIL
      description: |-
        Report - Profit and Loss Detail
        Method : GET

        Docs - https://developer.intuit.com/docs/api/accounting/profit%20and%20loss%20detail
      operationId: getReportsProfitandlossdetail
      x-api-path-slug: reportsprofitandlossdetail-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Profit
      - Loss
      - DETAIL
  /salesreceipt:
    post:
      summary: Post Sales Receipt
      description: |-
        Create an salesreceipt object
        Method : POST
      operationId: postSalesreceipt
      x-api-path-slug: salesreceipt-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Sales
      - Receipt
  /upload:
    post:
      summary: Post Upload
      description: "Uploading and linking new attachments\n\nhttps://developer.intuit.com/docs/0100_quickbooks_online/0200_dev_guides/accounting/attachments#Uploading_and_linking_new_attachments\n\nIf
        the attachment is not in the Attachment list already, it's possible to upload
        it and link it to the object in one multipart operation.\n\nOperation:      POST
        https://quickbooks.api.intuit.com/v3/company/companyID/upload\nContent type:
        multipart/form-data\n\nRequest body\n\nThe following sample code shows the
        multipart request body for uploading a file and its supporting Attachable
        metatdata object, with the result of it being both added to the Attachment
        list and added to the object.\n\nThe Attachable object accompanying this request
        supplies metadata and object information to which the attachment is linked.
        \nEach part of the multipart request is separated by a boundary.  In the sample
        below, the string  --YOjcLaTlykb6OxfYJx4O07j1MweeMFem is used.  You can use
        any random and unique string.\nThe file to be uploaded and its Attachable
        object are paired together via the name parameter in the part header for each
        one.\nThe name parameter for the file part is of the form file_content_nn,
        where nn is a unique index number among the set of files being uploaded.\nThe
        name parameter for the Attachable object is of the form file_metadata_nn,
        where nn corresponds to the file index number used with the content .\nThe
        file or files are stored in the Attachment list with the name specified by
        the filename parameter.\nIf the data supplied with the Attachable object cannot
        be validated, an error is returned and the file is not uploaded."
      operationId: postUpload
      x-api-path-slug: upload-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Upload
  /customer:
    post:
      summary: Post Customer
      description: |-
        Create a customer
        Method : POST
      operationId: postCustomer
      x-api-path-slug: customer-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Customer
  /department:
    post:
      summary: Post Department
      description: |-
        Create a department object
        Method : POST
      operationId: postDepartment
      x-api-path-slug: department-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Department
  /reports/GeneralLedger:
    get:
      summary: Get Reports General Ledger
      description: |-
        Report - General Ledger
        Method : GET

        Docs - https://developer.intuit.com/docs/api/accounting/general%20ledger
      operationId: getReportsGeneralledger
      x-api-path-slug: reportsgeneralledger-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - General
      - Ledger
  /reports/VendorBalance:
    get:
      summary: Get Reports Vendor Balance
      description: "Report - Vendor Balance \nMethod : GET\n\nDocs - https://developer.intuit.com/docs/api/accounting/vendor%20balance"
      operationId: getReportsVendorbalance
      x-api-path-slug: reportsvendorbalance-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Vendor
      - Balance
  /purchaseorder/178:
    get:
      summary: Get Purchase Order
      description: |-
        Read a puchase-order object
        Method : POST
      operationId: getPurchaseorder178
      x-api-path-slug: purchaseorder178-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Purchase
      - Order
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---