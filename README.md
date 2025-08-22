# LED Lights Payback Calculator

A comprehensive, self-contained web-based calculator for comparing LED lighting solutions and calculating ROI/payback periods. This calculator runs entirely in the browser with no external dependencies.

## 🚀 Features

### Core Functionality

- **Baseline vs Proposed Comparison**: Compare current lighting with LED alternatives
- **Product Catalog Dropdown**: 24 pre-configured LED fixtures with auto-populated wattage
- **Real-time Calculations**: Instant ROI and payback period updates
- **Responsive Design**: Works on all devices and screen sizes
- **Data Persistence**: Saves user inputs locally for convenience

### Product Catalog

The calculator includes your complete product line:

#### Tundra Area Light Series

- 70W, 100W, 150W, 200W, 240W, 300W

#### Orbix Round UFO Light Series

- 70W, 100W, 150W, 180W, 200W, 240W

#### Alpine LED Wall Pack Light Series

- 80W, 100W, 120W

#### Raven Backlit Flat Panel Light Series

- **2x4 Series**: 30W, 40W, 50W, 60W, 72W
- **2x2/1x4 Series**: 15W, 20W, 25W, 30W, 40W

### Calculations

- **Annual Energy Usage**: `Quantity × Watts × Hours × 365 ÷ 1000`
- **Annual Energy Cost**: `Annual Energy × (Rate ÷ 100)`
- **Initial Cost**: `Quantity × Cost per Fixture`
- **Annual Savings**: `Baseline Cost - Proposed Cost`
- **Payback Period**: `Proposed Initial Cost ÷ Annual Savings`
- **ROI**: `(Annual Savings ÷ Initial Cost) × 100`
- **10-Year Savings**: `Annual Savings × 10`

## 📱 Responsive Design

- **Desktop**: Full two-column layout with side-by-side comparison
- **Tablet**: Responsive grid that adapts to medium screens
- **Mobile**: Single-column layout optimized for touch interaction
- **Print**: Clean print styles for professional reports

## 🎨 Design Features

- **Modern UI**: Clean, professional interface inspired by industry standards
- **Color Coding**: Blue for baseline, green for proposed, red for savings
- **Interactive Elements**: Hover effects, focus states, and smooth transitions
- **Accessibility**: High contrast, readable fonts, and keyboard navigation

## 🚀 Deployment

### WordPress Integration

1. Copy the entire contents of `led-payback-calculator.html`
2. In WordPress, add a "Custom HTML" block
3. Paste the HTML code
4. Publish your page

### Other CMS Platforms

- **Drupal**: Use the "Custom HTML" block or "PHP Code" block
- **Joomla**: Use the "Custom HTML" module
- **Squarespace**: Use the "Code" block
- **Wix**: Use the "HTML" widget

### Direct File Upload

1. Upload `led-payback-calculator.html` to your web server
2. Access via direct URL
3. No additional setup required

## 🔧 Customization

### Company Branding

To add your company logo and branding:

1. **Replace the header title**:

   ```html
   <h1>Your Company Name - LED Calculator</h1>
   ```

2. **Add company logo**:

   ```html
   <div class="header">
     <img
       src="path/to/your/logo.png"
       alt="Company Logo"
       style="height: 50px;"
     />
     <h1>LED Lights Payback Calculator</h1>
     <!-- ... rest of header ... -->
   </div>
   ```

3. **Update colors** (in the CSS section):
   ```css
   .header {
     background: linear-gradient(
       135deg,
       #YOUR_PRIMARY_COLOR,
       #YOUR_SECONDARY_COLOR
     );
   }
   ```

### Product Catalog Updates

To add new products or modify existing ones, edit the `productCatalog` array in the JavaScript section:

```javascript
const productCatalog = [
  // Add your new products here
  {
    id: "new-product",
    name: "New Product Name",
    watts: 100,
    category: "Category Name",
  },
];
```

## 📊 Usage Instructions

### For End Users

1. **Enter General Parameters**:

   - Set electricity rate (cents/kWh)
   - Set operation hours per day

2. **Configure Baseline**:

   - Enter current lighting description
   - Specify quantity, watts per fixture, and cost

3. **Select Proposed Solution**:

   - Choose from the product dropdown
   - Enter quantity and cost per fixture
   - Wattage auto-populates from selection

4. **Review Results**:
   - Compare costs and energy usage
   - See annual savings and payback period
   - View 10-year projections

### For Administrators

- **Add Control**: Integrate with lighting control systems
- **Add Rebate**: Include available incentives and rebates
- **Print Results**: Generate professional reports

## 🧪 Testing

The calculator has been tested on:

- **Browsers**: Chrome, Safari, Firefox, Edge (latest versions)
- **Devices**: Desktop, tablet, mobile
- **Screen Sizes**: 320px to 1920px+
- **Print**: Chrome and Safari print preview

## 📁 File Structure

```
led-payback-calculator.html  # Main calculator file
README.md                     # This documentation
PRD.md                       # Product requirements document
```

## 🔒 Security & Privacy

- **No External Requests**: All functionality is self-contained
- **Local Storage**: User data is saved locally in the browser
- **No Backend**: No server-side processing or data collection
- **Client-Side Only**: All calculations happen in the user's browser

## 🆘 Troubleshooting

### Common Issues

1. **Calculator not loading**: Ensure JavaScript is enabled
2. **Styling issues**: Check for CSS conflicts with your theme
3. **Mobile responsiveness**: Test on actual devices, not just browser dev tools

### Browser Compatibility

- **Chrome**: 90+ (Full support)
- **Safari**: 14+ (Full support)
- **Firefox**: 88+ (Full support)
- **Edge**: 90+ (Full support)

## 📈 Future Enhancements

Potential features for future versions:

- **Multiple Baseline Scenarios**: Compare multiple current setups
- **Advanced Controls**: Dimming, scheduling, and sensor integration
- **Export Options**: PDF, Excel, and CSV export
- **Multi-language Support**: Internationalization
- **Advanced Analytics**: Detailed energy consumption patterns

## 📞 Support

For technical support or customization requests:

- Review this documentation thoroughly
- Check browser console for JavaScript errors
- Test in different browsers and devices
- Ensure no CSS conflicts with your website theme

## 📄 License

This calculator is provided as-is for your business use. Modify and customize as needed for your specific requirements.

---

**Last Updated**: December 2024  
**Version**: 1.0  
**Compatibility**: All modern browsers and devices
# led-roi-calculator
