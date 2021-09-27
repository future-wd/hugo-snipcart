upgrade to 3.2.1  
create public module
create readme.md   
set version to 3.2.0 then add the following update:
implement dependabot here or in the parent repo??


{{ partial "snipcart/hints" . }}

<link rel="preconnect" href="https://app.snipcart.com">
<link rel="preconnect" href="https://cdn.snipcart.com">


{{ partial "snipcart/css" . }}
<link rel="stylesheet" href="https://cdn.snipcart.com/themes/v3.2.1/default/snipcart.css" />



{{ partial "snipcart/js" "YOUR_PUBLIC_API_KEY" }}
<script async src="https://cdn.snipcart.com/themes/v3.2.1/default/snipcart.js"></script>
<div hidden id="snipcart" data-api-key="{{ . }}"></div>