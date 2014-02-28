# AngularJS Phonegap Push Notifications

## Usage

1. Made sure the `phonegap.js` script is in your `.html` file.
2. Replace {your_sender_id} with your GCM sender id
3. Include the `push.js` script, and this script's dependencies are included in your app.
4. Add `phonegap` as a module dependency to your app.

## Example

    push.registerPush(function (result) {
        if (result.type === 'registration') {
            console.log("PUSh Registrazione device_id:"+result.id+" Device:"+result.device);
        }else{
            console.log("PUSH errore");
        }
    });

## License
MIT
