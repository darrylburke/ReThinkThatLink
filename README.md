
*ReThinkThatLink**
----
  The ReThink Thank Link api allows you to obtain the same (and more) information about the resolution of a Short URL. Note: the API is rate limited, please play nice ;)

* **URL**

  https://rethinkthatlink.com/index.php

* **Method:**

  `GET`
  
*  **URL Params**

   **Required:**
 
   `url=[url encoded string]`

* **Data Params**

  None

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `[See Sample Below]`
 
* **Error Response:**

  * **Code:** 404 NOT FOUND <br />
  

  

* **Sample Retun:**

  ```
  {
    "src_url": "http:\/\/bit.ly\/QtQET",
    "Copyright": "Short URL Security Checker \u00a9 Burke Consulting 2017",
    "src_https": false,
    "contains_redirect": true,
    "destinations": [
        {
            "id": 0,
            "src_url": "http:\/\/bit.ly\/QtQET",
            "contains_redirect": true,
            "redirect_url": "http:\/\/bit.ly",
            "external_destination": false,
            "dl_time": 0.025364,
            "content_type": "text\/html; charset=utf-8",
            "ssl_verify_result": 0,
            "size_download": 100,
            "primary_ip": "67.199.248.11",
            "ssl_verify_result_errors": false,
            "page_http_status": 301,
            "cookies": {
                "_bit": "h95dOf-64285566ec8e2a5546-00a"
            },
            "uses_cookies": true,
            "redirect_threat_score": 4,
            "redirect_threat_score_reasons": "Contains a Redirect and Uses Cookies[+3];Redirects to HTTP[+1];"
        },
        {
            "id": 1,
            "src_url": "http:\/\/bit.ly",
            "contains_redirect": true,
            "redirect_url": "https:\/\/bitly.com\/",
            "external_destination": true,
            "dl_time": 0.018681,
            "content_type": "text\/html",
            "ssl_verify_result": 0,
            "size_download": 154,
            "primary_ip": "67.199.248.11",
            "ssl_verify_result_errors": false,
            "page_http_status": 302,
            "cookies": [

            ],
            "uses_cookies": false,
            "redirect_threat_score": 1,
            "redirect_threat_score_reasons": "Contains a Redirect[+1];External Destination[+2];BONUS Score: Redirects from  HTTP to HTTPS[-1]];"
        },
        {
            "id": 2,
            "src_url": "https:\/\/bitly.com\/",
            "contains_redirect": false,
            "dl_time": 0.085232,
            "content_type": "text\/html; charset=UTF-8",
            "ssl_verify_result": 0,
            "size_download": 7295,
            "primary_ip": "67.199.248.14",
            "ssl_verify_result_errors": false,
            "page_http_status": 200,
            "cookies": {
                "_xsrf": "2de125a67bc84e82a05841884df6c37e",
                "anon_u": "cHN1X19lNmNmZGFiNS1iOGRhLTQ3MWQtODZhZC02MThjMDlkYWRkMDQ=|1507211415|533e6dd36878811ca3ba41cb5c9d9d3af93f5c46"
            },
            "uses_cookies": true,
            "redirect_threat_score": 0,
            "redirect_threat_score_reasons": ""
        }
    ],
    "final_url": "https:\/\/bitly.com\/",
    "min_external_threat_score": 1,
    "max_external_threat_score": 1,
    "avg_external_threat_score": 0.33333333333333,
    "sum_external_threat_score": 1,
    "api_calls": 7
}
  ```
