# ![LOGO](logo.png) Api2Pdf - PDF Generation, Powered by AWS Lambda MSP Connector

## Description

A generated MSP connector for the Api2Pdf - PDF Generation, Powered by AWS Lambda API (version 1.0.0).

Generated from: https://api.apis.guru/v2/specs/api2pdf.com/1.0.0/openapi.json<br/>
Generated at: 2019-05-07T11:16:57+03:00

## API Description


# Introduction
[Api2Pdf](https://www.api2pdf.com) is a powerful PDF generation API with no rate limits or file size constraints. Api2Pdf runs on AWS Lambda, a serverless architecture powered by Amazon to scale to millions of requests while being up to 90% cheaper than alternatives. **Supports wkhtmltopdf, Headless Chrome, LibreOffice, and PDF Merge.** You can also generate barcodes with ZXING (Zebra Crossing).
# SDKs & Client Libraries
We've made a number of open source libraries available for the API
- Python: [https://github.com/api2pdf/api2pdf.python](https://github.com/api2pdf/api2pdf.python)
- .NET: [https://github.com/api2pdf/api2pdf.dotnet](https://github.com/api2pdf/api2pdf.dotnet)
- Nodejs: [https://github.com/api2pdf/api2pdf.node](https://github.com/api2pdf/api2pdf.node)
- PHP: [https://github.com/Api2Pdf/api2pdf.php](https://github.com/Api2Pdf/api2pdf.php)
- Ruby: (Coming soon)
# Authorization
Create an account at [portal.api2pdf.com](https://portal.api2pdf.com/register) to get an API key.

**Authorize your API calls**
- GET requests, include apikey=YOUR-API-KEY as a query string parameter
- POST requests, add **Authorization** to your header.
``` Authorization: YOUR-API-KEY ```

# Quickstart
If you are looking for just a quick call to grab PDFs of a URL, you can do a GET request like:
``` https://v2018.api2pdf.com/chrome/url?url={UrlToConvert}&apikey={YourApiKey} ```

For more advanced usage and settings, see the API specification below.


## Authorization

Supported authorization schemes:
- API Key- API Key
## Actions

### Convert raw HTML to PDF

> Convert HTML to a PDF using Headless Chrome on AWS Lambda.<br/>
> ### Authorize via Header of Request<br/>
> **Authorization: YOUR-API-KEY**

*Tags:* `Headless Chrome`

### Convert URL to PDF

> Convert a URL or Web Page to PDF using Headless Chrome on AWS Lambda. This GET request is for convenience and does not support advanced options. Use the POST request for more flexibility.<br/>
> ### Authorize via Query String Parameter<br/>
> **apikey=YOUR-API-KEY**<br/>
> ### Example<br/>
> ``` https://v2018.api2pdf.com/chrome/url?url={UrlToConvert}&apikey={YourApiKey} ```

*Tags:* `Headless Chrome`

#### Input Parameters
* `url` - _required_ - Url of the page to convert to PDF. Must start with http:// or https://.
* `output` - _optional_ - Specify output=json to receive a JSON output. Defaults to PDF file.

### Convert URL to PDF

> Convert a URL or Web Page to PDF using Headless Chrome on AWS Lambda..<br/>
> ### Authorize via Header of Request<br/>
> **Authorization: YOUR-API-KEY**

*Tags:* `Headless Chrome`

### Convert office document or image to PDF

> Convert an office document (Word, Excel, Powerpoint) or an image (jpg, gif, png) to a PDF using LibreOffice on AWS Lambda.<br/>
> ### Authorize via Header of Request<br/>
> **Authorization: YOUR-API-KEY**

*Tags:* `LibreOffice`

### Merge multiple PDFs together

> Merge two or more PDFs together on AWS Lambda.<br/>
> ### Authorize via Header of Request<br/>
> **Authorization: YOUR-API-KEY**

*Tags:* `Merge / Combine Pdfs`

### Convert raw HTML to PDF

> Convert HTML to a PDF using WkHtmlToPdf on AWS Lambda.<br/>
> ### Authorize via Header of Request<br/>
> **Authorization: YOUR-API-KEY**

*Tags:* `wkhtmltopdf`

### Convert URL to PDF

> Convert a URL or Web Page to PDF using WkHtmlToPdf on AWS Lambda. This GET request is for convenience and does not support advanced options. Use the POST request for more flexibility.<br/>
> ### Authorize via Query String Parameter<br/>
> **apikey=YOUR-API-KEY**<br/>
> ### Example<br/>
> ``` https://v2018.api2pdf.com/wkhtmltopdf/url?url={UrlToConvert}&apikey={YourApiKey} ```

*Tags:* `wkhtmltopdf`

#### Input Parameters
* `url` - _required_ - Url of the page to convert to PDF. Must start with http:// or https://.
* `output` - _optional_ - Specify output=json to receive a JSON output. Defaults to PDF file.

### Convert URL to PDF

> Convert a URL or Web Page to PDF using WkHtmlToPdf on AWS Lambda..<br/>
> ### Authorize via Header of Request<br/>
> **Authorization: YOUR-API-KEY**

*Tags:* `wkhtmltopdf`

### Generate bar codes and QR codes with ZXING.

> See full list of options and documentation [here](https://www.api2pdf.com/documentation/advanced-options-zxing-zebra-crossing-barcodes/)<br/>
> ### Authorize via Query String Parameter<br/>
> **apikey=YOUR-API-KEY**<br/>
> ### Example<br/>
> ``` https://v2018.api2pdf.com/zebra?format={format}&apikey={YourApiKey}&value={YourText} ```

*Tags:* `ZXING (Zebra Crossing) Bar Codes`

#### Input Parameters
* `format` - _required_ - Most common is CODE_39 or QR_CODE
* `value` - _required_ - Specify the text value you want to convert
* `showlabel` - _optional_ - Show label of text below barcode
* `height` - _optional_ - Height of the barcode generated image
* `width` - _optional_ - Width of the barcode generated image

## License

flowground :- Telekom iPaaS / api-2-pdf-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
