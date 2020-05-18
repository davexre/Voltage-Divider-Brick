# Voltage Divider Brick

This is a small board that implements a [voltage divider](https://en.wikipedia.org/wiki/Voltage_divider), making it easy to keep high voltages off a processor board,
like an Arduino. It's inspired by ElecFreaks Octopus bricks. They used to make a voltage divider brick much like this
one - in fact, I own one and am using it with my [Induction Annealer](https://github.com/davexre/Annealer-v3-PCB) project. 
In trying to help some other folks set their annealers up for Arduino control, I noticed that Octopus' bricks are no longer
available, and there's not a brick-like board out there that easily fills the gap. So, I put this one together.

The design changes are really that I chose to use axial resistors (to make assembly and repair easier), and I changed the
input connector to a 5mm pitch version that allows wire sizes up to 12AWG. 

### Build of Materials

- 1x [CUI Devices TB001-500-02BE](https://www.mouser.com/ProductDetail/CUI-Devices/TB001-500-02BE?qs=vLWxofP3U2zBBnHgU5u3DA%3D%3D)
- 1x [Molex 22-23-2021](https://www.mouser.com/ProductDetail/molex/22-23-2021/?qs=ILqg114nvd4YKlRlbo3yMg%3D%3D&countrycode=US&currencycode=USD)
- 2 appropriate resistors

### Resistor choices

You can choose whatever resistors make sense to you. Normally, for best results, precision resistors would be recommended for
this role. The original Octopus board divided the input voltage by 16, so R1 was 15kOhm, and R2 was 1kOhm. Mouser has equivalent
axial resistors available for both:

- [1 kOhm - .1% 15PPM 1/4W](https://www.mouser.com/ProductDetail/TE-Connectivity-Neohm/YR1B1K0CC?qs=sGAEpiMZZMtlubZbdhIBIIvX6HIFvcbFzVJZ4ENBTC8%3D)
- [15 kOhm - .1% 15PPM 1/4/W](https://www.mouser.com/ProductDetail/TE-Connectivity-Neohm/YR1B15KCC?qs=VHcS2MTj4gZfAJSm%2FAKdUg%3D%3D)

### Connectors

J1 can really be any .1" pitch connector you wish to use. The Molex connector indicated includes polarity and a locking
feature, but you could solder directly to it, or use normal breakaway header pins, or anything else you like. 
