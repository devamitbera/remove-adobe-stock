# 🧩 Remove Adobe Stock Modules for Magento Open Source

This package safely removes **Adobe Stock-related modules** from **Magento Open Source** installations.  
Since Adobe Stock integration is rarely used in most Magento stores, removing it helps make your setup **lighter**, **faster**, and **cleaner**.

---

## 🎯 Why Remove Adobe Stock?

Magento Open Source includes several **Adobe Stock** modules that are primarily designed for **Adobe Commerce (Enterprise)**.  
For most Magento stores, these modules are unnecessary and can:

- Increase dependency load  
- Slow down deployments and compilation  
- Introduce unused admin UI components  

Removing them improves performance and simplifies maintenance.

---

## ⚙️ Modules Removed

This package removes or replaces the following modules:

- `magento/module-adobe-ims`  
- `magento/module-adobe-ims-api`  
- `magento/module-adobe-stock-admin-ui`  
- `magento/module-adobe-stock-asset-api`  
- `magento/module-adobe-stock-client`  
- `magento/module-adobe-stock-client-api`  
- `magento/module-adobe-stock-image`  
- `magento/module-adobe-stock-image-admin-ui`  
- `magento/module-adobe-stock-image-api`

---

## 🚀 Installation

### Option 1: Composer (recommended)

```bash
composer require devamitbera/remove-adobe-stock
```

After installation, run the following commands to clean and update your setup:

```bash
bin/magento setup:upgrade
bin/magento setup:di:compile
bin/magento cache:flush
```

You can verify that Adobe modules are removed by running:

```bash
#bin/magento module:status | grep Adobe
```

---

---

## 💡 Benefits

✅ Reduces unused dependencies  
✅ Speeds up setup and compilation  
✅ Improves admin performance  
✅ Keeps your Magento Open Source installation clean and optimized  

---

## 🧾 Compatibility

| Magento Version | Supported |
|------------------|------------|
| 2.4.4 - 2.4.7-p9 | ✅ Tested |
| Adobe Commerce (EE) | ⚠️ Not recommended |

---

## 👨‍💻 Author

**Amit Bera**  
Owner of [amitbera.com](https://amitbera.com)  
Magento Developer & DevOps Engineer  
Moderator on [Magento Stack Exchange](https://magento.stackexchange.com/users/57367/amit-bera)  

- 🔗 [GitHub Profile](https://github.com/devamitbera)  
- 📨 [Open an Issue](../../issues) for support or suggestions  
- ⭐ Star the repository if you found it useful!

---

## 🪪 License

This project is licensed under the [MIT License](LICENSE).

---

> 💬 *“A lighter Magento is a faster Magento.”*
