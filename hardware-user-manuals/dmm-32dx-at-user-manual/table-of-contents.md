# TABLE OF CONTENTS

[1.DESCRIPTION ](1.-description.md)

[2. FEATURES ](2.-features.md)

[3. DMM-32DX-AT BOARD DRAWING](3.-dmm-32dx-at-board-drawing.md) 

[4. I/O HEADERS PINOUT AND PIN DESCRIPTION ](4.-i-o-headers-pinout-and-pin-description/)

      [4.1 Analog I/O Header – J3 ](4.-i-o-headers-pinout-and-pin-description/4.1-analog-i-o-header-j3.md)

      [4.2 Digital I/O Header – J4 ](4.-i-o-headers-pinout-and-pin-description/4.2-digital-i-o-header-j4.md)

      [4.3 Serial I/O Header – J11 ](4.-i-o-headers-pinout-and-pin-description/4.3-serial-i-o-header-j11.md)

[5. BOARD CONFIGURATION ](5.-board-configuration/)

      [5.1 Base Address ](5.-board-configuration/5.1-base-address.md)

      [5.2 Interrupt level](5.-board-configuration/5.2-interrupt-level.md) 

      [5.3 DMA level ](5.-board-configuration/5.3-dma-level.md)

     [ 5.4 Single-Ended / Differential A/D Channels ](5.-board-configuration/5.4-single-ended-differential-a-d-channels.md)

      [5.5 D/A Configuration ](5.-board-configuration/5.5-d-a-configuration.md)

      [5.6 Digital I/O Pull-Up / Pull-Down ](5.-board-configuration/5.6-digital-i-o-pull-up-pull-down.md)

    [  5.7 16-Bit Data Bus](5.-board-configuration/5.7-16-bit-data-bus.md) 

[6. I/O REGISTER MAP ](6.-i-o-register-map/)

      [6.1 I/O Map Description ](6.-i-o-register-map/6.1-i-o-map-description.md)

      [6.2 I/O Map Reference – Write, I/O Map Reference – Read ](6.-i-o-register-map/untitled-2.md)

[      6.3 I/O Map Details ](6.-i-o-register-map/untitled-3.md)

[      6.4 Page 0: 82C54 Counter/Timer Access ](6.-i-o-register-map/untitled-5.md)

[      6.5 Page 1: 82C55 Digital I/O Circuit ](6.-i-o-register-map/untitled-6.md)

[      6.6 Page 2: Expanded FIFO Control ](6.-i-o-register-map/untitled-7.md)

[      6.7 Page 3: Autocalibration Registers ](6.-i-o-register-map/untitled-1.md)

[      6.8 Page 4: dsPIC Interface ](6.-i-o-register-map/6.8-page-4-dspic-interface.md)

[      6.9 Page 5: D/A Waveform Generator ](6.-i-o-register-map/6.9-page-5-d-a-waveform-generator.md)

[      6.10 Page 6: CPLD I/O Window ](6.-i-o-register-map/6.10-page-6-cpld-i-o-window.md)

[      6.11 Page 7: D/A Output Channel Control ](6.-i-o-register-map/6.11-page-7-d-a-output-channel-control.md)

[7. ENABLING ENHANCED FEATURES ](untitled/)

[      7.1 Enabling Enhanced Features \(Enhanced Mode\) ](untitled/7.1-enabling-enhanced-features-enhanced-mode.md)

[      7.2 Disabling Enhanced Features \(Normal Mode\) ](untitled/7.2-disabling-enhanced-features-normal-mode.md)

[8. ANALOG INPUT RANGES AND RESOLUTION ](8.-analog-input-ranges-and-resolution/)

[      8.1 Unipolar and Bipolar Inputs ](8.-analog-input-ranges-and-resolution/8.1-unipolar-and-bipolar-inputs.md)

[      8.2 Input Ranges and Resolution ](8.-analog-input-ranges-and-resolution/8.2-input-ranges-and-resolution.md)

[      8.3 A/D Conversion Formulas ](8.-analog-input-ranges-and-resolution/8.3-a-d-conversion-formulas.md)

[      8.4 Correlation between A/D Code and Input Voltage ](8.-analog-input-ranges-and-resolution/8.4-correlation-between-a-d-code-and-input-voltage.md)

[9. PERFORMING AN A/D CONVERSION ](9.-performing-an-a-d-conversion/)

[      9.1 Select the input channel or input channel range ](9.-performing-an-a-d-conversion/9.1-select-the-input-channel-or-input-channel-range.md)

[      9.2 Select the analog input range ](9.-performing-an-a-d-conversion/9.2-select-the-analog-input-range.md)

[      9.3 Wait for the analog circuit to settle ](9.-performing-an-a-d-conversion/9.3-wait-for-the-analog-circuit-to-settle.md)

[      9.4 Start an A/D conversion on the current channel ](9.-performing-an-a-d-conversion/9.4-start-an-a-d-conversion-on-the-current-channel.md)

[      9.5 Wait for the conversion to finish ](9.-performing-an-a-d-conversion/9.5-wait-for-the-conversion-to-finish.md)

[      9.6 Read the A/D data ](9.-performing-an-a-d-conversion/9.6-read-the-a-d-data.md)

[      9.7 Convert the numerical data to a meaningful value](9.-performing-an-a-d-conversion/9.7-convert-the-numerical-data-to-a-meaningful-value.md)

[ 10. A/D SAMPLING METHODS ](10.a-d-sampling-methods/)

[      10.1 Sampling Modes ](10.a-d-sampling-methods/10.1-sampling-modes.md)

[      10.2 FIFO Description ](10.a-d-sampling-methods/10.2-fifo-description.md)

[      10.3 Scan Sampling ](10.a-d-sampling-methods/10.3-scan-sampling.md)

[      10.4 Sequential Sampling ](10.a-d-sampling-methods/10.4-sequential-sampling.md)

[11. HOW TO PERFORM A/D CONVERSIONS USING INTERRUPTS ](11.how-to-perform-a-d-conversions-using-interrupts.md)

[12. ANALOG OUTPUT RANGES AND RESOLUTION ](12.-analog-output-ranges-and-resolution/)

[       12.1 Description ](12.-analog-output-ranges-and-resolution/12.1-description.md)

[       12.2 Resolution ](12.-analog-output-ranges-and-resolution/12.2-resolution.md)

[       12.3 Full-Scale Range Selection ](12.-analog-output-ranges-and-resolution/12.3-full-scale-range-selection.md)

[13. GENERATING AN ANALOG OUTPUT ](13.generating-an-analog-output/)

[       13.1 Compute the D/A code for the desired output voltage ](13.generating-an-analog-output/13.1-compute-the-d-a-code-for-the-desired-output-voltage.md)

[       13.2 Compute the LSB and MSB values ](13.generating-an-analog-output/13.2-compute-the-lsb-and-msb-values.md)

[       13.3 Add the channel number to the MSB ](13.generating-an-analog-output/13.3-add-the-channel-number-to-the-msb.md)

[       13.4 Set D/A Simultaneous Update bit ](13.generating-an-analog-output/13.4-set-d-a-simultaneous-update-bit.md)

[       13.5 Write the LSB and MSB to the board ](13.generating-an-analog-output/13.5-write-the-lsb-and-msb-to-the-board.md)

[       13.6 Monitor the DACBUSY status bit ](13.generating-an-analog-output/13.6-monitor-the-dacbusy-status-bit.md)

[14. D/A WAVEFORM GENERATOR ](14.d-a-waveform-generator/)

[        14.1 Description ](14.d-a-waveform-generator/14.1-description.md)

[        14.2 Programming the D/A wave form generator ](14.d-a-waveform-generator/14.2-programming-the-d-a-wave-form-generator.md)

[        14.3 Enable enhanced features ](14.d-a-waveform-generator/14.3-enable-enhanced-features.md)

[        14.4 Reset D/A wave form pointer ](14.d-a-waveform-generator/14.4-reset-d-a-wave-form-pointer.md)

[        14.5 Latch D/A value ](14.d-a-waveform-generator/14.5-latch-d-a-value.md)

[        14.6 Store D/A values into buffer ](14.d-a-waveform-generator/14.6-store-d-a-values-into-buffer.md)

[        14.7 Setup D/A wave form settings ](14.d-a-waveform-generator/14.7-setup-d-a-wave-form-settings.md)

[        14.8 Start D/A waveform generator ](14.d-a-waveform-generator/14.8-start-d-a-waveform-generator.md)

[15. AUTOCALIBRATION ](15.autocalibration.md)

[16. DIGITAL I/O OPERATION ](16.digital-i-o-operation/)

[        16.1 Main Digital I/O on J4: Internal 82C55 Circuit ](16.digital-i-o-operation/16.1-main-digital-i-o-on-j4-internal-82c55-circuit.md)

[        16.2 Digital I/O Configuration Register ](16.digital-i-o-operation/16.2-digital-i-o-configuration-register.md)

[        16.3 Mode 0 Digital I/O ](16.digital-i-o-operation/16.3-mode-0-digital-i-o.md)

[         16.4 Mode 1 Digital I/O With Handshaking ](16.digital-i-o-operation/16.4-mode-1-digital-i-o-with-handshaking.md)

[         16.5 Auxiliary Digital I/O on J3 ](16.digital-i-o-operation/16.5-auxiliary-digital-i-o-on-j3.md)

[17. COUNTER/TIMER OPERATION ](17.counter-timer-operation/)

[         17.1 Counter/Timer Features and Configuration Options ](17.counter-timer-operation/17.1-counter-timer-features-and-configuration-options.md)

[         17.2 Counter/Timer Configuration ](17.counter-timer-operation/17.2-counter-timer-configuration.md)

[         17.3 Counter/Timer Access and Programming ](17.counter-timer-operation/17.3-counter-timer-access-and-programming.md)

[18. SPECIFICATIONS](18.specifications.md)

