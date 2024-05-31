# Security

### **Security Considerations**

#### Secure Computing Environments

Moon Vault employs secure computing environments, notably Trusted Execution Environments (TEEs) and Confidential Containers, to provide a high level of security and confidentiality. The TEE, referred to as an enclave, is a protected memory region that ensures the confidentiality of data and code execution. Importantly, it does not require an operating system, effectively removing the OS vendor from the trusted compute base. This enhances the security by reducing potential vulnerabilities associated with the operating system.

In addition, Moon Vault uses Confidential Containers bringing confidential computing to Kubernetes containers. This ensures the entrypoint process of a container is executed inside a hardware-based TEE. It provides a safe environment that is shielded from other confidential containers and any hosting environment within the TEE. This combination of TEEs and Confidential Containers provides a secure, confidential, and reliable computing environment.



#### Pseudo-Randomness

Moon Vault takes advantage of the Entropy Augmentation to ensure the uniqueness of private key generation. This feature leverages an external Hardware Security Module (HSM) to augment system entropy via the PKCS#11 protocol, which is a widely accepted industry standard for interfacing with cryptographic tokens.

Pseudo-random generators, while useful, come with certain limitations. They generate sequences of numbers approximating the properties of random numbers, which means there is a possibility of repetition or patterns. This can be a critical issue when it comes to the generation of cryptographic keys, where uniqueness and unpredictability are paramount for security.

To address this, Moon Vault enhances the system entropy, which is the randomness collected by an operating system or application for use in cryptography or other uses that require random data. By augmenting entropy using an external HSM, Moon Vault can improve the randomness and thereby the security of the generated private keys. This approach significantly reduces the risk of key duplication or predictability.

#### Encryption in transit

Moon uses end-to-end encryption via HTTPS certificates to protect data. This method guarantees that data stays secure and private, even if intercepted during transmission.

#### Data Security

* **Root Key Wrapping**: Encrypts the root key using a Hardware Security Module (HSM) for enhanced protection, superior to key splitting.
* **Automatic Unsealing**: Stores the HSM-encrypted root key in Vault, enabling automatic access to encrypted data at startup, enhancing convenience without sacrificing security.
* **Seal Wrapping**: Complies with Federal Information Processing Standards (FIPS) for secure storage of Critical Security Parameters, adding an extra layer of data protection.

#### Session security

* **JWTs with Short Expiry**: Prevents token misuse by expiring quickly.
* **Immediate Session Revocation**: Enhances security by promptly revoking compromised sessions.
* **MFA Claims in Tokens**: Adds an extra layer of user verification.
* **Comprehensive Security**: Ensures only authorized users access sessions and swiftly addresses threats.

#### Development security

* **Automated Security Scanning**: Uses tools like Dependabot to quickly identify and fix vulnerabilities, maintaining system integrity.
* **Rigorous Testing**: Ensures all features meet quality standards, enhancing system performance and reliability.
* **CI/CD Pipeline**: Streamlines development, facilitating effective integration and faster software updates.
* **Code Reviews**: Ensures code meets standards and best practices, catching potential issues early.
