# hack_code

```
private void init() {
        WebSettings mWebSettings = getSettings();
        mWebSettings.setSupportZoom(true);
        mWebSettings.setDefaultTextEncodingName("utf-8");
        mWebSettings.setLoadsImagesAutomatically(true);
        mWebSettings.setAllowFileAccessFromFileURLs(true);
        mWebSettings.setAllowUniversalAccessFromFileURLs(true);
        mWebSettings.setJavaScriptEnabled(true);
        mWebSettings.setDomStorageEnabled(true);

        setWebViewClient(webViewClient);
        setWebChromeClient(webChromeClient);
    }
 ```
    
 ```
      public void clearSetting(){
        loadDataWithBaseURL(null, "", "text/html", "utf-8", null);
        clearHistory();
        clearCache(true);
        setWebChromeClient(null);
        setWebViewClient(null);
    }
 ```
