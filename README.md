# Knockout.underscore plugin
This plugin adds all Underscore array methods(and object/array methods) to Observable Array.

Use it like you would with a normal array, the only difference is that you need to skip the first argument(which is the array).
Example:

    var VM = {
      arr: ko.observableArray(["bill","ted","rufus"])
    };

    alert(VM.arr.min(function(n){
       return n.length;
    }));

    //prints "ted"

Also, there are 11 new destructive methods that change the observable array:

* .select_
* .reject_
* .invoke_
* .sortBy_
* .rest_
* .compact_
* .flatten_
* .without_
* .uniq_
* .intersect_
* .zip_

See Underscore.js documentation for more details.

