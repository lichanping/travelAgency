# Travel Agency Workspace Instructions

## Hotel price research
- Do not access Google or Google Hotels for this project. The user has no VPN; do not assume or attempt to use a VPN.
- Prefer Chrome DevTools MCP for browser-based hotel research in this project.
- When the user requests current hotel prices, use directly accessible booking providers only (for example, Booking.com, Trip.com, or Ctrip). Do not substitute search-result snippets, cached guide prices, or generic starting prices for a live quote.
- Use the itinerary's actual check-in/check-out dates and the stated party size. Unless the user changes it, compare one room for two adults, with taxes included where the provider shows a total.
- The travelers are coworkers: require a twin room explicitly described as two single beds. Do not accept double/king/semi-double beds, unspecified bed assignments, or futons as equivalent. A Twin room name alone is not sufficient evidence.
- Always label breakfast inclusion and smoking/non-smoking status, or explicitly mark them unknown. Neither breakfast nor non-smoking is a mandatory filter.
- Display and record prices in RMB/CNY so the user can compare them easily. If the provider only shows another currency, convert using a current, stated exchange rate and retain the provider's original amount and currency as the source value.
- For each quote, record the provider, query date, room/meal conditions when shown, RMB total and tax status, and cancellation terms. Distinguish unavailable rooms from prices that could not be checked.
- If a provider is inaccessible, region-blocked, or requires unavailable login/verification, report that limitation. Do not bypass it, use Google, infer a price, or write an unverified amount into the itinerary.
- In the itinerary HTML, preserve the previous quote using `<del>` and show a verified current quote in red. Include the source and query date near the updated price; do not present a historical quote as current.
