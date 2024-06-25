# Email and password

### Authentication Methods

The `MoonSDK` class provides the following authentication methods:

#### 1. Email and Password Authentication

The `signUp` and `signInWithPassword` methods allow users to create an account or sign in using their email address and password. Here's how to use them:

<pre class="language-javascript"><code class="lang-javascript">import { MoonSDK } from '@moonup/moon-sdk';

<strong>const moonSDK = new MoonSDK(config);
</strong>
async function signUpWithEmailAndPassword(email, password) {
  try {
    await moonSDK.signUp(email, password);
    console.log('Account created successfully.');
  } catch (error) {
    console.error('Error creating account:', error);
  }
}

async function signInWithEmailAndPassword(email, password) {
  try {
    await moonSDK.signInWithPassword(email, password);
    console.log('Signed in successfully.');
  } catch (error) {
    console.error('Error signing in:', error);
  }
}
</code></pre>

#### 2. Phone Number Authentication

The `signInWithPhone` method allows users to sign in using their phone number and password. Here's how to use it:

```javascript
import { MoonSDK } from '@moonup/moon-sdk';

const moonSDK = new MoonSDK(config);

async function signInWithPhone(phone, password) {
  try {
    await moonSDK.signInWithPhone(phone, password);
    console.log('Signed in successfully.');
  } catch (error) {
    console.error('Error signing in:', error);
  }
}
```
