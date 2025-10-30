# ☕️ Cafe Curator 🍵

A modern web application that helps users discover and save their favorite cafes nearby using geolocation and the Google Places API.

## Features

- **Location-Based Search**: Automatically finds cafes near your current location
- **Swipe Interface**: Tinder-style card swiping interface to browse cafes
- **Save Favorites**: Swipe right to save cafes you're interested in
- **Offline Access**: View saved cafes even without internet connection
- **Location Caching**: Saves location data for 10 minutes to reduce API calls
- **Responsive Design**: Works on both desktop and mobile devices

## Technologies Used

- HTML5 Geolocation API
- Google Places API for cafe data
- HammerJS for touch/swipe gestures
- Local Storage for saving favorites
- Custom CSS for card-based UI
- Savate font family for typography

## Setup

1. **Clone the repository**

2. **API Key Setup:**
   - Get a Google Places API key from [Google Cloud Console](https://console.cloud.google.com/)
   - Replace `YOUR_API_KEY` in `index.html` with your actual API key:
   ```javascript
   const apiKey = "YOUR_API_KEY";
   ```

3. **CORS Proxy:**
   - The app uses a CORS proxy to handle API requests
   - You can disable it by setting `useProxy = false` if not needed
   - Or use your own proxy service by modifying the `proxy` constant

## Usage

1. Open `index.html` in a modern web browser
2. Click "Find Cafes Near Me" to start discovering cafes
3. Allow location access when prompted
4. Swipe right to save cafes you like
5. Swipe left to dismiss
6. Click "Show Saved Cafes" to view your saved locations

## Features Details

### Location Cards
- Display cafe name
- Show rating (if available)
- Include photo from Google Places
- Smooth swipe animations
- Stacked card layout

### Local Storage
- Saves favorite cafes
- Caches location data
- Persists between sessions
- Prevents duplicate saves

## Styling

The app features a clean, modern design with:
- Light green background
- Custom font integration
- Responsive card layouts
- Smooth transitions and animations
- Mobile-friendly interface

## Security Notes

- API key should be properly secured in production
- Uses HTTPS for API requests
- Implements basic error handling
- Location data is temporarily cached

## Browser Support

Works best in modern browsers with support for:
- ES6+ JavaScript
- CSS Grid/Flexbox
- Touch events
- Local Storage
- Geolocation API

## Contributing

Feel free to fork and submit pull requests. Please ensure you:
1. Maintain consistent code style
2. Test thoroughly
3. Document any new features
4. Update README as needed

## License

MIT License - Feel free to use and modify as needed.