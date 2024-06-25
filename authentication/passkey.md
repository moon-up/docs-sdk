# Passkey

## WebAuthn in MoonSDK

WebAuthn is a web standard published by the World Wide Web Consortium (W3C) that enables passwordless logins on the web. It allows users to use local authenticators (such as biometrics or FIDO2 devices) to securely authenticate to web applications. MoonSDK uses WebAuthn to provide a secure and user-friendly authentication method.

### React WebAuthn Component

Here's a simplified example of a React component that uses WebAuthn for registration and login using the MoonSDK class functions:

```javascript
import React, { useState } from 'react';
import { startAuthentication, startRegistration } from '@simplewebauthn/browser';
import { MoonSDK } from '@moonup/moon-sdk';

const sdk = new MoonSDK();

function WebAuthnComponent() {
  const [email, setEmail] = useState('');

  const handleLogin = async () => {
    const auth = await sdk.handlePassKeyLogin(email);
    const credential = await startAuthentication(auth);
    const response = await sdk.handlePasskeyLoginVerify(email, credential);
  };

  const handleRegister = async () => {
    const options = await sdk.handleRegister(email);
    const credential = await startRegistration(options);
    const token = await sdk.handleRegisterVerify(email, credential, options);
  };

  return (
    <div>
      <input type="email" onChange={(e) => setEmail(e.target.value)} />
      <button onClick={handleLogin}>Login with WebAuthn</button>
      <button onClick={handleRegister}>Register with WebAuthn</button>
    </div>
  );
}

export default WebAuthnComponent;
```

This component includes an input field for the user's email and two buttons for login and registration. When the user clicks on the login or register button, the corresponding handler function is called. These functions use the MoonSDK class functions to interact with the server and the user's authenticator. After the user has authenticated with their authenticator, the credential is sent to the server for verification.

### WebAuthn in MoonSDK

WebAuthn in MoonSDK provides a secure and user-friendly authentication method. By using local authenticators, users can log in to web applications without remembering and typing passwords. MoonSDK's React WebAuthn component simplifies the integration of WebAuthn into your application, allowing users to easily register and log in using their authenticators.

### Benefits of WebAuthn in MoonSDK

* Security: WebAuthn provides strong security guarantees, making it a secure choice for authentication.
* User-friendly: WebAuthn allows users to log in using local authenticators, such as biometrics or FIDO2 devices, making the authentication process more user-friendly.
* Simplified integration: MoonSDK's React WebAuthn component simplifies the integration of WebAuthn into your application, making it easy to add WebAuthn support to your project.

### Conclusion

WebAuthn is a powerful authentication method that provides strong security guarantees and a user-friendly experience. MoonSDK's React WebAuthn component simplifies the integration of WebAuthn into your application, making it easy to add WebAuthn support to your project. Whether you're building a new application or looking to improve the security and usability of an existing one, WebAuthn in MoonSDK is a great choice.
