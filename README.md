🌟  Star_Velocity  🌟

This Python script is part of an ongoing college project that analyzes stellar spectra and estimates the projected rotational velocity (𝑣 sin 𝑖) of a star using Fourier Transform techniques. It's worth nothing that this is not the final version, for I'd like it to be able to automatically compute the next plot after selecting the points of reference.


📖 Description

The code processes spectral data from a star and a Gaussian profile to:

    Convert wavelength data to velocity space.

    Select and isolate spectral lines of interest.

    Perform Fourier Transform (FFT) on both the star's spectral line and the Gaussian.

    Compare the resulting Fourier spectra to determine the star's projected rotational velocity (v sin i).


📂 Files Required

    StarsData.txt — observed spectral data (wavelength vs flux).

    gaussian.dat — theoretical Gaussian profile (velocity vs normalized flux).


🛠 Installation

Clone the repository:

  git clone https://github.com/Joule-sCode/Star_Velocity.git
  
  cd Star_Velocity

Install the required Python libraries:

  pip install numpy matplotlib scipy


📈 How It Works

    Wavelength → Velocity: Converts wavelength data relative to the line center into a velocity scale.

    Spectral Line Selection: Zooms into a specific line by selecting velocity limits.

    Data Preparation: Adds continuum parts to the Gaussian and star data for cleaner Fourier Transform results.

    FFT Analysis: Performs Fast Fourier Transform (FFT) and identifies key frequencies related to rotational broadening.

    v sin i Calculation: Based on the ratio of Fourier frequencies between the Gaussian and stellar data.


🤝 Contributing

Pull requests are welcome!
If you have suggestions for improvements or new features, feel free to open an issue.


📄 License

This project is licensed under the MIT License.
  
