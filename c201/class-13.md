# Local Storage

## cookies

- early use for persistent **local storage**
  
- slows down your web application by transmitting same data
- sending data unencrypted over the internet
- limited to about 4 KB of data

## HTML5 Storage

- Way for web pages to store *key/values* locally within the browser

- data stays after you navigate away from the browser

### Check for html5 Storage

```js

function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}
```

<cite>http://diveinto.html5doctor.com/storage.html<cite>

### Using HTML5 Storage

- Use a named key to access storage

- All data coming out will be a string

- you can treat this storage like a associative array

### How to clear storage area

```js
interface Storage {
  deleter void removeItem(in DOMString key);
  void clear();
};

```

### Limitations

- 5 megabytes of storage
- Cannot ask user for more space