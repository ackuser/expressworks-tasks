Your submission results compared to the expected:

                 ACTUAL                                 EXPECTED
────────────────────────────────────────────────────────────────────────────────

   "<h1>Hello World</h1><p>Today is Mon Dec 21 2015.</p>" ==    "<h1>Hello World</h1><p>Today is Mon Dec 21 2015.</p>"

────────────────────────────────────────────────────────────────────────────────

✓ Submission results match expected

# PASS

Your solution to JADE passed!

Here's the official solution in case you want to compare notes:

────────────────────────────────────────────────────────────────────────────────
    var express = require('express')
    var app = express()
    app.set('view engine', 'jade')
    app.set('views', process.argv[3])
    app.get('/home', function(req, res) {
      res.render('index', {date: new Date().toDateString()})
    })
    app.listen(process.argv[2])

────────────────────────────────────────────────────────────────────────────────

You have 5 challenges left.
Type 'expressworks' to show the menu.
