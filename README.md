# pasarguard-sdk

pasarguard-sdk is a fully typed TypeScript client for interacting with the [Pasarguard](https://github.com/PasarGuard/panel) API.
It provides a clean, consistent, and developer-friendly interface — with built-in authentication, retries, and WebSocket support.
Based on [Marzban SDK](https://github.com/Ilmar7786/marzban-sdk).

## 📦 Installation

Install PasarGuardSDK via npm:

```sh
npm install pasarguard-sdk
```

Or using yarn:

```sh
yarn add pasarguard-sdk
```

## Versions
Version of library is aligned with pasarguard panel version

## 📑 Configuration Options

The `Config` object is used to initialize the PasarGuardSDK instance. Below are all available options:

| Name                 | Type    | Required | Default | Description                                                                                        |
| -------------------- | ------- | -------- | ------- | -------------------------------------------------------------------------------------------------- |
| `baseUrl`            | string  | Yes      | —       | The base URL of the PasarGuard API instance. Example: `https://api.example.com`                       |
| `username`           | string  | Yes      | —       | The username for authentication.                                                                   |
| `password`           | string  | Yes      | —       | The password for authentication.                                                                   |
| `token`              | string  | No       | —       | Optional JWT token for direct authorization. If provided, SDK uses this token for requests.        |
| `retries`            | number  | No       | 3       | Number of automatic retries for failed HTTP requests.                                              |
| `authenticateOnInit` | boolean | No       | true    | If true (default), SDK authenticates automatically on init. If false, call `authorize()` manually. |

---

## 🚀 Quick Start

```typescript
import { PasarGuardSDK } from '@assetsfirst/pasarguard-sdk'

const sdk = new PasarguardSDK({
  baseUrl: 'https://api.example.com',
  username: 'your-username',
  password: 'your-password',
})

// Fetch user details
const username = 'admin';
try {
  const user = await sdk.user.getUser(username);
  return {...user, expire: toUnixTimestamp(user.expire)};
} catch (e) {
  logger.warn(`A user with username ${username} is missing`);
  return undefined;
}


```
