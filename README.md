# 🌍 Awesome Open Data APIs

A **community-driven collection of free & open APIs** with examples.  
Perfect for developers, students, and hobbyists looking to build projects.  

👉 Goal: Make it easy for anyone to discover useful APIs and learn how to use them.  

---

## 📂 Categories

### 📈 Finance
- [Polygon.io](https://polygon.io) – Free stock & crypto data API (✅ Free tier, 🔑 Requires API Key)  
- [Frankfurter](https://www.frankfurter.app/) – Currency exchange rates, no auth required (✅ Free, 🚫 No Auth)
- [Invokely](https://invokely.ai/docs) - Official economic statistics for AI agents over MCP, with source citations on every figure. Free account: 500 MCP calls/month; REST data queries require Builder, Pro or prepaid credits. (✅ Free MCP tier, 🔑 API Key/OAuth; no-account trial: 25 calls/day/IP)

### 🌦️ Weather
- [Open-Meteo](https://open-meteo.com/) – Global weather forecasts (✅ Free, 🚫 No Auth)  
- [WeatherAPI](https://www.weatherapi.com/) – Weather and astronomy data (✅ Free tier, 🔑 API Key)

### 🛰️ Space
- [NASA Open APIs](https://api.nasa.gov/) – Space imagery, Mars Rover, and more (✅ Free, 🔑 API Key)  
- [Open Notify](http://open-notify.org/) – ISS location and astronaut data (✅ Free, 🚫 No Auth)

---

## 📖 Examples

We include code samples in `/examples` to help you get started quickly.  

Example in Python:
```python
import requests

response = requests.get("https://api.open-meteo.com/v1/forecast?latitude=35&longitude=139&hourly=temperature_2m")
data = response.json()
print(data["hourly"]["temperature_2m"][:5])
````

Example in JavaScript:

```javascript
fetch("https://api.open-meteo.com/v1/forecast?latitude=35&longitude=139&hourly=temperature_2m")
  .then(res => res.json())
  .then(data => console.log(data.hourly.temperature_2m.slice(0, 5)));
```

---

## 🤝 Contributing

We welcome contributions from everyone! 🎉

To add a new API:

1. Fork this repo
2. Edit `README.md` and add your API under the right category
3. (Optional) Add structured JSON entry in `/apis/`
4. Submit a Pull Request 🚀

See [CONTRIBUTING.md](CONTRIBUTING.md) for full details.

---

## 🛡️ Code of Conduct

Please check out our [Code of Conduct](CODE_OF_CONDUCT.md) to ensure a welcoming and inclusive environment.

---

## ⭐ Support

If you like this project, please consider giving it a **star** ⭐ on GitHub.
This helps others discover it and keeps the community growing!

````

---

 📄 `CONTRIBUTING.md`
 🤝 Contributing Guidelines

Thanks for considering contributing to **Awesome Open Data APIs**! 🎉  

We want this project to be **welcoming, beginner-friendly, and useful** for everyone.  

---

  🚀 How to Contribute

  1. Fork & Clone
- Fork this repository  
- Clone your fork locally:
  
  git clone https://github.com/YOUR_USERNAME/awesome-open-data-apis.git
````

### 2. Add an API

* Open `README.md`
* Add your API under the correct category with this format:

```
- [API Name](https://link-to-api.com) – Short description (✅ Free / 🔑 Requires API Key / 🚫 No Auth)
```

👉 Example:

```
- [Dog CEO](https://dog.ceo/dog-api/) – Random dog images (✅ Free, 🚫 No Auth)
```

* (Optional) Add a JSON file under `/apis/` if you want to provide structured data:

```json
{
  "name": "Dog CEO",
  "url": "https://dog.ceo/dog-api/",
  "category": "Animals",
  "auth": "None",
  "free": true,
  "description": "Random dog images"
}
```

### 3. Run Checks

* Make sure your formatting is consistent.
* Keep descriptions short (max 1–2 lines).

### 4. Commit & Push

```bash
git checkout -b add-new-api
git commit -m "Added Dog CEO API under Animals"
git push origin add-new-api
```

### 5. Submit a Pull Request

* Open a PR to the `main` branch.
* Add a short description of what you changed.

---

## 💡 Contribution Tips

* Don’t worry if you’re new to GitHub—this repo is beginner-friendly!
* Even fixing typos, broken links, or improving examples is super helpful.
* If you’re unsure where to put an API, just make your best guess—we’ll help in review.

---

## 🛡️ Code of Conduct

Please follow our [Code of Conduct](CODE_OF_CONDUCT.md). We want this project to be a safe space for everyone.

---

Happy contributing! 🚀
