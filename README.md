# Promisify-functions-

function promiseFooFn(options) {
 return new Promise((resolve, reject) =>
 fooFn(options, (err, result) =>
 // If there's an error, reject; otherwise resolve
 err ? reject(err) : resolve(result)
 )
 );
}
