Chapters ([Linear Systems and Signals (Lathi)](https://annas-archive.gl/md5/4e15e058430c801865a53d6d9126dd02))
- 2 Time-domain Analysis of Continuous-time Systems
    - 2.1 Introduction
    - 2.2 System Response to Internal Conditions: The Zero-Input Response
        - 2.2-1 Some Insights into the Zero-Input Behavior of a System
    - 2.3 The Unit Impulse Response h(t)
    - 2.4 System Response to External Input: The Zero-State Response
        - 2.4-1 The Convolution Integral
        - 2.4-2 Graphical Understanding of Convolution Operation
        - 2.4-3 Interconnected Systems
        <!-- - 2.4-4 A Very Special Function for LTIC Systems: The Everlasting Exponential est
        - 2.4-5 Total Response -->
    <!-- - 2.5 System Stability
        - 2.5-1 External (BIBO) Stability
        - 2.5-2 Internal (Asymptotic) Stability
        - 2.5-3 Relationship Between BIBO and Asymptotic Stability
    - 2.6 Intuitive Insights into System Behavior
        - 2.6-1 Dependence of System Behavior on Characteristic Modes
        - 2.6-2 Response Time of a System: The System Time Constant
        - 2.6-3 Time Constant and Rise Time of a System
        - 2.6-4 Time Constant and Filtering
        - 2.6-5 Time Constant and Pulse Dispersion (Spreading)
        - 2.6-6 Time Constant and Rate of Information Transmission
        - 2.6-7 The Resonance Phenomenon
    - 2.7 MATLAB: M-Files
        - 2.7-1 Script M-Files
        - 2.7-2 Function M-Files 214viii   Contents
        - 2.7-3 For-Loops
        - 2.7-4 Graphical Understanding of Convolution
    - 2.8 Appendix: Determining the Impulse Response
    - 2.9 Summary
        - References
        - Problems -->

Videos:
- [Lecture 3 & Recitation 3: Feedback, Poles, and Fundamental Modes](https://ocw.mit.edu/courses/6-003-signals-and-systems-fall-2011/resources/lecture-3-feedback-poles-and-fundamental-modes/)
- [Lecture 4 & Recitation 4: Continuous-Time (CT) Systems](https://ocw.mit.edu/courses/6-003-signals-and-systems-fall-2011/resources/lecture-4-continuous-time-ct-systems/)

<!-- - 3 TIME-DOMAIN ANALYSIS OF DISCRETE-TIME SYSTEMS
    - 3.1 Introduction
        - 3.1-1 Size of a Discrete-Time Signal
    - 3.2 Useful Signal Operations
    - 3.3 Some Useful Discrete-Time Signal Models
        - 3.3-1 Discrete-Time Impulse Function δ[n]
        - 3.3-2 Discrete-Time Unit Step Function u[n]
        - 3.3-3 Discrete-Time Exponential γ n
        - 3.3-4 Discrete-Time Sinusoid cos (n + θ )
        - 3.3-5 Discrete-Time Complex Exponential ejn
    - 3.4 Examples of Discrete-Time Systems
        - 3.4-1 Classification of Discrete-Time Systems
    - 3.5 Discrete-Time System Equations
        - 3.5-1 Recursive (Iterative) Solution of Difference Equation
    - 3.6 System Response to Internal Conditions: The Zero-Input Response
    - 3.7 The Unit Impulse Response h[n]
        - 3.7-1 The Closed-Form Solution of h[n]
    - 3.8 System Response to External Input: The Zero-State Response
        - 3.8-1 Graphical Procedure for the Convolution Sum
        - 3.8-2 Interconnected Systems
        - 3.8-3 Total Response
    - 3.9 System Stability
        - 3.9-1 External (BIBO) Stability
        - 3.9-2 Internal (Asymptotic) Stability
        - 3.9-3 Relationship Between BIBO and Asymptotic Stability
    - 3.10 Intuitive Insights into System Behavior
    - 3.11 MATLAB: Discrete-Time Signals and Systems
        - 3.11-1 Discrete-Time Functions and Stem Plots
        - 3.11-2 System Responses Through Filtering
        - 3.11-3 A Custom Filter Function
        - 3.11-4 Discrete-Time Convolution
    - 3.12 Appendix: Impulse Response for a Special Case
    - 3.13 Summary
        - Problems

4 CONTINUOUS-TIME SYSTEM ANALYSIS USING THE LAPLACE TRANSFORM
    4.1 The Laplace Transform
        4.1-1 Finding the Inverse Transform
    4.2 Some Properties of the Laplace Transform
        4.2-1 Time Shifting
        4.2-2 Frequency Shifting
        4.2-3 The Time-Differentiation Property
        4.2-4 The Time-Integration Property
        4.2-5 The Scaling Property
        4.2-6 Time Convolution and Frequency Convolution
    4.3 Solution of Differential and Integro-Differential Equations
        4.3-1 Comments on Initial Conditions at 0− and at 0+
        4.3-2 Zero-State Response
        4.3-3 Stability
        4.3-4 Inverse Systems
    4.4 Analysis of Electrical Networks: The Transformed Network
        4.4-1 Analysis of Active Circuits
    4.5 Block Diagrams
    4.6 System Realization
        4.6-1 Direct Form I Realization
        4.6-2 Direct Form II Realization
        4.6-3 Cascade and Parallel Realizations
        4.6-4 Transposed Realization
        4.6-5 Using Operational Amplifiers for System Realization
    4.7 Application to Feedback and Controls
        4.7-1 Analysis of a Simple Control System
    4.8 Frequency Response of an LTIC System
        4.8-1 Steady-State Response to Causal Sinusoidal Inputs
    4.9 Bode Plots
        4.9-1 Constant Ka1 a2 /b1 b3
        4.9-2 Pole (or Zero) at the Origin
        4.9-3 First-Order Pole (or Zero)
        4.9-4 Second-Order Pole (or Zero)
        4.9-5 The Transfer Function from the Frequency Response
    4.10 Filter Design by Placement of Poles and Zeros of H(s)
        4.10-1 Dependence of Frequency Response on Poles and Zeros of H(s)
        4.10-2 Lowpass Filters
        4.10-3 Bandpass Filters
        4.10-4 Notch (Bandstop) Filters
        4.10-5 Practical Filters and Their Specifications
    4.11 The Bilateral Laplace Transform 445x   Contents
        4.11-1 Properties of the Bilateral Laplace Transform
        4.11-2 Using the Bilateral Transform for Linear System Analysis
    4.12 MATLAB: Continuous-Time Filters
        4.12-1 Frequency Response and Polynomial Evaluation
        4.12-2 Butterworth Filters and the Find Command
        4.12-3 Using Cascaded Second-Order Sections for Butterworth Filter Realization
        4.12-4 Chebyshev Filters
    4.13 Summary
        References
        Problems


5 DISCRETE-TIME SYSTEM ANALYSIS USING THE z-TRANSFORM
    5.1 The z-Transform
        5.1-1 Inverse Transform by Partial Fraction Expansion and Tables
        5.1-2 Inverse z-Transform by Power Series Expansion
    5.2 Some Properties of the z-Transform
        5.2-1 Time-Shifting Properties
        5.2-2 z-Domain Scaling Property (Multiplication by γ n )
        5.2-3 z-Domain Differentiation Property (Multiplication by n)
        5.2-4 Time-Reversal Property
        5.2-5 Convolution Property
    5.3 z-Transform Solution of Linear Difference Equations
        5.3-1 Zero-State Response of LTID Systems: The Transfer Function
        5.3-2 Stability
        5.3-3 Inverse Systems
    5.4 System Realization
    5.5 Frequency Response of Discrete-Time Systems
        5.5-1 The Periodic Nature of Frequency Response
        5.5-2 Aliasing and Sampling Rate
    5.6 Frequency Response from Pole-Zero Locations
    5.7 Digital Processing of Analog Signals
    5.8 The Bilateral z-Transform
        5.8-1 Properties of the Bilateral z-Transform
        5.8-2 Using the Bilateral z-Transform for Analysis of LTID Systems
    5.9 Connecting the Laplace and z-Transforms
    5.10 MATLAB: Discrete-Time IIR Filters
        5.10-1 Frequency Response and Pole-Zero Plots
        5.10-2 Transformation Basics
        5.10-3 Transformation by First-Order Backward Difference
        5.10-4 Bilinear Transformation
        5.10-5 Bilinear Transformation with Prewarping
        5.10-6 Example: Butterworth Filter Transformation
        5.10-7 Problems Finding Polynomial Roots
        5.10-8 Using Cascaded Second-Order Sections to Improve Design
    5.11 Summary
        References
        Problems

6 CONTINUOUS-TIME SIGNAL ANALYSIS: THE FOURIER SERIES
    6.1 Periodic Signal Representation by Trigonometric Fourier Series
        6.1-1 The Fourier Spectrum
        6.1-2 The Effect of Symmetry
        6.1-3 Determining the Fundamental Frequency and Period
    6.2 Existence and Convergence of the Fourier Series
        6.2-1 Convergence of a Series
        6.2-2 The Role of Amplitude and Phase Spectra in Waveshaping
    6.3 Exponential Fourier Series
        6.3-1 Exponential Fourier Spectra
        6.3-2 Parseval’s Theorem
        6.3-3 Properties of the Fourier Series
    6.4 LTIC System Response to Periodic Inputs
    6.5 Generalized Fourier Series: Signals as Vectors
        6.5-1 Component of a Vector
        6.5-2 Signal Comparison and Component of a Signal
        6.5-3 Extension to Complex Signals
        6.5-4 Signal Representation by an Orthogonal Signal Set
    6.6 Numerical Computation of Dn
    6.7 MATLAB: Fourier Series Applications
        6.7-1 Periodic Functions and the Gibbs Phenomenon
        6.7-2 Optimization and Phase Spectra
    6.8 Summary
        References
        Problems

7 CONTINUOUS-TIME SIGNAL ANALYSIS: THE FOURIER TRANSFORM
    7.1 Aperiodic Signal Representation by the Fourier Integral
        7.1-1 Physical Appreciation of the Fourier Transform
    7.2 Transforms of Some Useful Functions
        7.2-1 Connection Between the Fourier and Laplace Transforms
    7.3 Some Properties of the Fourier Transform
    7.4 Signal Transmission Through LTIC Systems
        7.4-1 Signal Distortion During Transmission
        7.4-2 Bandpass Systems and Group Delay 726xii   Contents

    7.5 Ideal and Practical Filters
    7.6 Signal Energy
    7.7 Application to Communications: Amplitude Modulation
        7.7-1 Double-Sideband, Suppressed-Carrier (DSB-SC) Modulation
        7.7-2 Amplitude Modulation (AM)
        7.7-3 Single-Sideband Modulation (SSB)
        7.7-4 Frequency-Division Multiplexing
    7.8 Data Truncation: Window Functions
        7.8-1 Using Windows in Filter Design
    7.9 MATLAB: Fourier Transform Topics
        7.9-1 The Sinc Function and the Scaling Property
        7.9-2 Parseval’s Theorem and Essential Bandwidth
        7.9-3 Spectral Sampling
        7.9-4 Kaiser Window Functions
    7.10 Summary
        References
        Problems


8 SAMPLING: THE BRIDGE FROM CONTINUOUS TO DISCRETE
    8.1 The Sampling Theorem
        8.1-1 Practical Sampling
    8.2 Signal Reconstruction
        8.2-1 Practical Difficulties in Signal Reconstruction
        8.2-2 Some Applications of the Sampling Theorem
    8.3 Analog-to-Digital (A/D) Conversion
    8.4 Dual of Time Sampling: Spectral Sampling
    8.5 Numerical Computation of the Fourier Transform:
        The Discrete Fourier Transform
        8.5-1 Some Properties of the DFT
        8.5-2 Some Applications of the DFT
    8.6 The Fast Fourier Transform (FFT)
    8.7 MATLAB: The Discrete Fourier Transform
        8.7-1 Computing the Discrete Fourier Transform
        8.7-2 Improving the Picture with Zero Padding
        8.7-3 Quantization
    8.8 Summary
        References
        Problems

9 FOURIER ANALYSIS OF DISCRETE-TIME SIGNALS
    9.1 Discrete-Time Fourier Series (DTFS)
        9.1-1 Periodic Signal Representation by Discrete-Time Fourier Series
        9.1-2 Fourier Spectra of a Periodic Signal x[n]
    9.2 Aperiodic Signal Representation
        by Fourier Integral
        9.2-1 Nature of Fourier Spectra
        9.2-2 Connection Between the DTFT and the z-Transform
    9.3 Properties of the DTFT
    9.4 LTI Discrete-Time System Analysis by DTFT
        9.4-1 Distortionless Transmission
        9.4-2 Ideal and Practical Filters
    9.5 DTFT Connection with the CTFT
        9.5-1 Use of DFT and FFT for Numerical Computation of the DTFT
    9.6 Generalization of the DTFT to the z-Transform
    9.7 MATLAB: Working with the DTFS and the DTFT
        9.7-1 Computing the Discrete-Time Fourier Series
        9.7-2 Measuring Code Performance
        9.7-3 FIR Filter Design by Frequency Sampling
    9.8 Summary
        Reference
        Problems

10 STATE-SPACE ANALYSIS
    10.1 Mathematical Preliminaries
        10.1-1 Derivatives and Integrals of a Matrix
        10.1-2 The Characteristic Equation of a Matrix: The Cayley–Hamilton Theorem
        10.1-3 Computation of an Exponential and a Power of a Matrix
    10.2 Introduction to State Space
    10.3 A Systematic Procedure to Determine State Equations
        10.3-1 Electrical Circuits
        10.3-2 State Equations from a Transfer Function
    10.4 Solution of State Equations
        10.4-1 Laplace Transform Solution of State Equations
        10.4-2 Time-Domain Solution of State Equations
    10.5 Linear Transformation of a State Vector
        10.5-1 Diagonalization of Matrix A
    10.6 Controllability and Observability
        10.6-1 Inadequacy of the Transfer Function Description of a System 953xiv   Contents
    10.7 State-Space Analysis of Discrete-Time Systems
            10.7-1 Solution in State Space
            10.7-2 The z-Transform Solution
    10.8 MATLAB: Toolboxes and State-Space Analysis
            10.8-1 z-Transform Solutions to Discrete-Time, State-Space Systems
            10.8-2 Transfer Functions from State-Space Representations
            10.8-3 Controllability and Observability of Discrete-Time Systems
            10.8-4 Matrix Exponentiation and the Matrix Exponential
    10.9 Summary
        References
        Problems -->