# Passkey

## WebAuthn in Moon

WebAuthn is a web standard published by the World Wide Web Consortium (W3C) for passwordless logins on the web. It allows users to use local authenticators (like biometrics or FIDO2 devices) to securely authenticate to web applications.

Moon uses WebAuthn to provide a secure and user-friendly authentication method. Instead of remembering and typing passwords, users can use their fingerprint, face recognition, or a security key to log in.

## React Webauthn Component

Here's a simplified example of a React component that uses WebAuthn for registration and login:

```tsx
import React, { useState } from 'react';
import { startAuthentication, startRegistration } from '@simplewebauthn/browser';

function WebAuthnComponent() {
  const [email, setEmail] = useState('');

  const handleLogin = async () => {
    const publicKey = await fetch('https://dash.usemoon.ai/api/webauthn/login', {
      method: 'POST',
      body: JSON.stringify({ email }),
      headers: { 'Content-Type': 'application/json' },
    }).then((res) => res.json());

    const credential = await startAuthentication(publicKey.optionsAuth);

    await fetch('https://dash.usemoon.ai/api/webauthn/login/verify', {
      method: 'POST',
      body: JSON.stringify({
        ...credential,
        username: email,
      }),
      headers: { 'Content-Type': 'application/json' },
    });
  };

  const handleRegister = async () => {
    const publicKey = await fetch('https://dash.usemoon.ai/api/webauthn/register', {
      method: 'POST',
      body: JSON.stringify({ email }),
      headers: { 'Content-Type': 'application/json' },
    }).then((res) => res.json());

    const credential = await startRegistration(publicKey.options);

    await fetch('https://dash.usemoon.ai/api/webauthn/register/verify', {
      method: 'POST',
      body: JSON.stringify({
        ...credential,
        email: email,
        user: {
          ...publicKey.options.user,
        },
      }),
      headers: { 'Content-Type': 'application/json' },
    });
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

This component includes an input field for the user's email and two buttons for login and registration. When the user clicks on the login or register button, the corresponding handler function is called. These functions communicate with the server to start the WebAuthn process and then use the `@simplewebauthn/browser` library to interact with the user's authenticator. After the user has authenticated with their authenticator, the credential is sent to the server for verification.
