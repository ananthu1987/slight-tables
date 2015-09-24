# Slight-Tables

Big data, small space - Slight Tables, a Bootstrap table plugin. Ever had a lot of data, lots of rows and lots of columns, but didn't have the screen real estate? Slight tables attempt to fix this problem. 

A demo is worth a thousand pictures: TODO: Add demo. 

## Setup

Import the scripts. 

```
<link href="bootstrap.css" rel="stylesheet" />
<link href="bootstrap.slight-tables.css" rel="stylesheet" />

<script src="jquery.js"></script>
<script src="bootstrap.js"></script>
<script src="bootstrap.slight-tables.js"></script>
```

Create a standard Bootstrap table. 

```
<div class="container">
    <div class="row">
            <table id="table" class="table table-striped">
                <thead>
                    <tr>
                        <th>Name</th>
                        <th>Company</th>
                        <th>Regional</th>
                        <th>Credit Card</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Cole</td>
                        <td>Mollis Non Cursus Foundation</td>
                        <td>Natalie</td>
                        <td>346580390287563</td>
                    </tr>
                </tbody>
            </table>
    </div>
</div>
```

Create a new `SlightTable`. 

```
<script>
$(function () {
    var selector = $("#table");
    var table = new SlightTable(selector, {
        "maxCols": 5, // Hide columns greater than this number
        maxRowOptions: [10, 20, 50, 100],
        resizable: false // Should it use the WebKit resizable feature. 
    });
});
</script>
```

## License 

Slight Tables is under the MIT license, pull requests and forks are welcome. 