BarcodeReader v2.0 for Web
==========================
This is a fork from https://github.com/EddieLa/JOB

BarcodeReader is a barcode reader for Code128, Code93, Code39, Standard/Industrial 2 of 5,
Interleaved 2 of 5, Codabar and EAN-13 barcodes in javascript.
Supports multiple barcodes in one image and detects what type of barcodes there are.

I've taken the web version of Eddie's demo and done some housekeeping a little bit. 
I've also made a simple function to setup the live stream barcode reader.

You can find the new demo here

https://iemadk.github.io/BarCode-reader

## How to use
Starter template

```HTML
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Document</title>
</head>

<body>
  <p id="code">code will appear here</p>

  <script src="https://code.jquery.com/jquery-3.3.1.min.js"></script>
  <script src="BarcodeScanner.js"></script>
  <script src="app.js"></script>
  <script>
    var resultElement = document.getElementById('code')
    setupLiveReader(resultElement)
  </script>
</body>

</html>
```