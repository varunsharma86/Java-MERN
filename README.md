# Java-MERN
myCollection.insertMany([
    {name: {first: "Andrew", last: "Morgan"},
    {name: {first: "Elvis"}, died: 1977},
    {name: {last: "Mainwaring", title: "Captain"}, born: 1885}
])
.then(
    function(results) {
        resolve(results.insertedCount);
    },
    function(err) {
        console.log("Failed to insert Docs: " + err.message);
        reject(err);
    }
)
