# PawsOrganization Project

## Description
This project is a web application containerized using Docker. It can be run locally for testing or deployed via Docker.
It contains details of an animal adoption website

---

## Design Decisions

### Color Palette
- Primary: `#123456`  
- Secondary: `#abcdef`  
- Accent: `#fedcba`  
- Background: `#f5f5f5`  
- Text: `#333333`

### Type Scale
- Headings: `H1: 36px`, `H2: 30px`, `H3: 24px`, `H4: 20px`, `H5: 18px`, `H6: 16px`  
- Body: `16px`  
- Small: `14px`  

### Spacing Scale
- XS: `4px`  
- S: `8px`  
- M: `16px`  
- L: `24px`  
- XL: `32px`  

### Components
- Buttons: primary, secondary, disabled states  
- Forms: input, textarea, select, error states  
- Cards: elevation, shadow, padding consistent with spacing scale  

---

## Accessibility Notes
- Color contrast checked to meet **WCAG AA standards**.  
- Focus styles visible for all interactive elements.  
- Reduced motion: animations respect `prefers-reduced-motion`.  

---

## Docker

### Build
```bash
docker build -t pawsorg .
docker tag pawsorg your-dockerhub-username/pawsorg:latest
docker push your-dockerhub-username/pawsorg:latest

