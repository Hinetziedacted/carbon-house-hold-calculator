## Household Carbon Calculator

A single-page, offline carbon footprint calculator for 6 regions with 10 inputs → annual/monthly footprint + 3 personalized tips.

**Live Demo:** https://YOUR_USERNAME.github.io/carbon-calculator/

## Features

**Region-specific electricity factors** (India, Finland, UK, EU, US, Global)  
**Transport modes** (personal vehicle, bus, flights with radiative forcing)  
**Diet types** (vegan, vegetarian, low-meat, high-meat)  
**100% client-side** – no APIs, no server, works offline  
**Mobile-responsive** – works on phone, tablet, desktop  

## How to Use

1. Open the calculator at the link above
2. Adjust the 10 input fields for your situation
3. Click **Calculate**
4. See your annual/monthly footprint, breakdown by category, and 3 actionable tips

## Emission Factors (Sources)

### Electricity (kg CO2e per kWh)
- **India:** 0.727 (CEA baseline 2023-24)
- **Finland:** 0.094 (low-carbon grid)
- **UK:** 0.225 (2024 generation + transmission)
- **EU (avg):** 0.255 (2022 data)
- **US:** 0.373 (EPA 2022 eGrid)
- **Global:** 0.45 (generic baseline)

### LPG Cooking Fuel (kg CO2e per kg)
- **India:** 3.13
- **Other regions:** 3.00

### Transport (kg CO2e per km or per passenger-km)
- **Two-wheeler (petrol):** 0.0516 kg/km
- **Small petrol car:** 0.148 kg/km
- **Bus/Metro:** 0.089 kg per passenger-km (DEFRA 2024)
- **Flights (all, incl. RF):** 0.2726 kg per passenger-km

### Diet (kg CO2e per person per year)
- **Vegan:** ~1,500 kg/yr
- **Vegetarian:** ~1,700 kg/yr
- **Low-meat:** ~1,900 kg/yr
- **High-meat:** ~3,300 kg/yr

## Calculation Method

Annual per-person footprint:
Electricity = (monthly_kWh - solar_kWh) × 12 × grid_factor ÷ household_size
LPG = monthly_lpg_kg × 12 × lpg_factor ÷ household_size
Vehicle = weekly_km × 52 × vehicle_factor
Bus = weekly_km × 52 × 0.089
Flights = annual_km × 0.2726
Diet = annual_preset

Total = Electricity + LPG + Vehicle + Bus + Flights + Diet
Monthly = Total ÷ 12


## Contributing

Please read [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) and [CONTRIBUTING.md](CONTRIBUTING.md) before opening issues or pull requests.

### How to Contribute
1. Fork the repository
2. Make changes in a new branch
3. Test locally by opening index.html in a browser
4. Submit a pull request with a clear description

## License

MIT License – see [LICENSE](LICENSE) for details.

## Citation

If you use this tool in research or projects, cite it as:

YourName. (2025). Household Carbon Calculator. GitHub.
https://github.com/YOUR_USERNAME/carbon-calculator



Or use the CITATION.cff file for automated citation generation.

## Sources & References

- CEA Carbon Baseline Database: https://cea.nic.in/
- DEFRA 2024 GHG Conversion Factors: https://gov.uk/
- EPA eGRID 2022: https://epa.gov/
- Our World in Data Diet Emissions: https://ourworldindata.org/
- Climatiq API: https://climatiq.io/
- Nowtricity (Finland grid): https://nowtricity.com/

---

**Questions?** Open an issue or check the CONTRIBUTING guidelines.

