# Day 6 — API + JSON + Debugging

## What I understood

API endpoints can need required authentication headers.  
If the required header is missing, the server returns an access error.

---

## 1. GET request

First, I made a GET request to the API and got JSON with a list of users.

![GET users](screenshots/api_get_users_response.png)

---

## 2. POST request without API key

I sent a POST request with `fetch` without the `x-api-key` header.

![POST without key](screenshots/api_post_without_key.png)

---

## 3. Error response

The server returned an error:

- `missing_api_key`
- `401 Unauthorized`

This means the endpoint needs a required authentication header.

![API error](screenshots/api_missing_key_error.png)

---

## 4. Fixed request

After that, I added `x-api-key` to the headers and sent the POST request again.

![POST with key](screenshots/api_post_with_key.png)

---

## 5. Success response

After the fix, the server processed the request successfully and returned a
correct JSON response.

![Success response](screenshots/api_success_response.png)

---

## 6. Changed JSON value

I changed the value of the `job` field and saw that the new value went to the
JSON body and showed in the response.

![Changed JSON value](screenshots/api_changed_job_value.png)

---

## Conclusion

I understood that an API can block requests without required authentication
headers.

I also saw a real debugging flow:

`GET → POST → 401 error → fix headers → success`

This helped me better understand how API authentication works and why headers
are important for access control.
