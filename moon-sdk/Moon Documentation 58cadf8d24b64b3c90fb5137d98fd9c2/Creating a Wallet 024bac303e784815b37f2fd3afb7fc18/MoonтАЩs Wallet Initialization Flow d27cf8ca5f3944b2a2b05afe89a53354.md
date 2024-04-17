# Moon’s Wallet Initialization Flow

> Moon wallet initialization begins with an authenticated user's create account request on the frontend triggering a backend callback. A backend HTTP request is sent to the create account API endpoint, initiating an HTTP response from the API endpoint back to the backend.
> 

![Untitled](Moon%E2%80%99s%20Wallet%20Initialization%20Flow%20d27cf8ca5f3944b2a2b05afe89a53354/Untitled.png)

> A unique JWT token is transferred from the Moon backend to the HaschorpVault, establishing a secure communication channel. The HashCorpVault utilizes this JWT token to authenticate and authorize the creation of a new wallet on the designated blockchain network. The HascorpVault generates a unique public and private key pair for the new wallet.
> 

![Untitled](Moon%E2%80%99s%20Wallet%20Initialization%20Flow%20d27cf8ca5f3944b2a2b05afe89a53354/Untitled%201.png)

> A wallet address is generated, incorporating the public key as a unique identifier for the wallet, and the underlying private key as the secure authentication mechanism for accessing and managing the wallet. The HascorpVault sends a response back to the Moon backend, including the generated wallet address link. Authenticated users can then access their newly created wallet using this address link via the frontend.
> 

![Untitled](Moon%E2%80%99s%20Wallet%20Initialization%20Flow%20d27cf8ca5f3944b2a2b05afe89a53354/Untitled%202.png)