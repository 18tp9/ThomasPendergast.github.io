<!DOCTYPE html>
<html lang="en">

<body>
    <header>
        <h1>VTFF</h1>
    </header>
    <p>In image processing for visual tracers, cutoff filters are often employed to isolate pixels in an intensity range associated with the presence of a tracer. This process often involves iteratively processing images with different cutoff values to determine the appropriate range. We introduce VTFF (Visual Tracer Filter Finder): a simple python application for interactive filter tuning in image processing. VTFF provides an interactive environment to view and assess in real-time the effect of changing filter parameters including high and low-pass filter values and median filtering window sizes. This application aims to expedite the filter tuning process and serve as a pre-processing step to determine filter parameter values prior to bulk processing.</p>
    <section>
        <h2>Capabilities</h2>
        <ul>
            <li>Parsing through images in directory </li>
            <li>Toggling on/off contours over the image being analyzed </li>
            <li>Adjusting cutoff/threshold filter pixel intensity range </li>
            <li>Toggling on/off median filter and changing window size </li>
        </ul>
    </section>
    <section>
        <h2>Instructions</h2>
        <p>The user will be prompted to select image directory upon running. They then will be promted to either select a background image or employ a maximum filter across the image directory as a proxy for background subtraction. Left and right arrows are used to parse through the images in the selected directory. Contours from the background subtraction will be shown over top of the image. Pressing 'c' prompts the user to input lower and upper cutoff pixel intensity values to isolate tune the filter for tracer isolation. Pressing the spacebar allows the user to toggle on and off the contours to determine if the cutoff filter is accurately capturing the extent of the visible tracer in the image. Lastly, pressing 'm' turns on a median filter and prompts the user to input a window size for the filter. This median filter can be turned off by pressing 'm' again and pressing enter or by setting the window size to zero.</p>
        <p>All code is found in VTFF.py and example images are provided in the "examples" folder.</p>
    </section>
</body>
</html>
