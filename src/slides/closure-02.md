# Closure

``` javascript
(function () {
  
  var Users = {
    list: [],

    getAll: function () {
      var self = this;
      $.post('/api/users.json').then(function (resp) {
        self.list = resp.users;
      });
    }
  }

  $(document).on('ready', function () {
    Users.getAll();
  });

})();
```

---