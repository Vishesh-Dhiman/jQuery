# Adding jQuery to a Web Page  

Web page me jQuery ko include karna bahut simple hai. Aap do tariko se jQuery ko apne project me use kar sakte ho:  

---

## 1. jQuery CDN ke through  
Content Delivery Network (CDN) ka use karke aap bina jQuery ko download kiye, directly apne HTML page me include kar sakte ho.  

### Steps:  
1. HTML file me `<head>` ya `<body>` ke andar jQuery ka CDN link add karo.  
2. Ye link directly jQuery ke hosted file ko load karega.  

### Example Code:  
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Add jQuery</title>
  <!-- jQuery CDN Link -->
  <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
</head>
<body>
  <h1>Welcome to jQuery</h1>
  <script>
    $(document).ready(function() {
      alert("jQuery is working!");
    });
  </script>
</body>
</html>
```

## Advantages of Using CDN:

- Fast loading speed because CDN servers are optimized.

- Browser cache kar leta hai, to baar-baar load nahi karna padta.

- No need to download the jQuery file.


---

## Downloaded jQuery File ke through

Agar aapke paas internet nahi hai ya aap offline kaam kar rahe ho, to jQuery file ko download karke use kar sakte ho.

### Steps:

1. Visit the jQuery Download Page.
2. Latest version ki jQuery file download karo (.min.js file recommended hai).
3. Apne project folder me jQuery file ko save karo (e.g., js folder me).
4. HTML file me <script> tag ke andar uska path specify karo.



## Example Code:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Add jQuery</title>
  <!-- Local jQuery File -->
  <script src="js/jquery-3.6.0.min.js"></script>
</head>
<body>
  <h1>Welcome to Offline jQuery</h1>
  <script>
    $(document).ready(function() {
      console.log("jQuery is loaded from a local file!");
    });
  </script>
</body>
</html>
```

## Advantages of Downloaded File:
- Offline usage.
- No dependency on internet speed or CDN availability.

---

## Conclusion

- Aapko apne project ke requirement ke hisaab se CDN ya downloaded file ka use karna chahiye.
- CDN faster hai aur hassle-free hota hai.
- Downloaded file aapke local setup ke liye convenient hai.
