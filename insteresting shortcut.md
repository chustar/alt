I just saw an interesting shortcut:  

    lastScope && lastScope.destroy();

If I were implementing this, I would probably have written it as:  

    if (lastScope) lastScope.destroy();

And I would have slapped myself on the back for being clever with the `if (lastScope)` (micro-)optimization.

After reading JavaScript Allongé, I might have written it as:  

    maybe('destroy')(lastScope);

with `maybe` defined as:  

    function maybe(funcName) { 
      return function(obj) { 
        if(obj) { 
          obj[funcName]() 
        }
      } 
    };
And then I would have congratulated myself for "thinking functionally" (No, I wouldn't actually write that).