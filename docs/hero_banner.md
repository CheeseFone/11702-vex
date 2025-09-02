PRD: VEX Robotics Club Hero Banner (HTML Implementation)
1. Overview

The hero banner is the introductory section of the VEX Robotics Club website, built with vanilla HTML, CSS, and JavaScript. It delivers a layered, parallax-scrolling effect combined with simple, blocky animations. The design will feel bold and playful, aligning with team branding, while staying lightweight and performant without any frameworks.

2. Objectives

Implement the hero using only HTML, CSS, and JavaScript.

Ensure the title image (title.jpg) is the first visible element.

Position the robot image (robot.jpg) slightly behind, scrolling faster for the parallax effect.

Stop the robot at a defined dead stop point, creating a transition moment.

Fade in exclamation animations (two-frame blocky swap at 1 fps).

Add other animated features (smiley animations).

Deliver smooth performance across devices without external libraries.

3. Key Features
3.1 Parallax Scroll

Layers:

Title (title.jpg) = foreground.

Robot (robot.jpg) = background, scrolls faster.

Behavior:

Title moves slower on scroll.

Robot moves faster until capped (dead stop).

Once robot locks, triggers exclamation fade-in.

3.2 Transition & Fade-in

Robot halts → exclamation section fades in.

Transition done with CSS opacity + transform.

Robot gets stronger drop shadow to emphasize the lock.

3.3 Exclamation Animation

Images: exclaimation_1.jpg, exclaimation_2.jpg.

Frame Rate: 1 frame per second, using JS setInterval().

Style: Blocky → image-rendering: pixelated.

Trigger: Starts only after robot settles.

3.4 Smiley Animation

Images: smiley_1.jpg, smiley_2.jpg.

Frame Rate: 1 fps, synced with exclamation.

Position: Sticky in viewport corner (e.g., top-right).

Extra Motion: Float animation via CSS keyframes.

4. Design & Aesthetic

Color Palette: Red #d71920, Black #0a0a0a, White #ffffff.

Visual Mood: Minimal, bold, dynamic.

Layout:

Centered hero images.

Responsive sizing with max-width + clamp().

Accessibility:

Respect prefers-reduced-motion: disable parallax and frame swaps, but show static exclamation.

5. Technical Requirements
5.1 Stack

HTML5 for structure.

CSS3 for styling, transitions, and floating animation.

Vanilla JavaScript for:

Parallax transform calculations.

Sprite swapping at 1 fps.

Fade-in triggers.

5.2 Parallax Logic

Attach scroll listener.

Use requestAnimationFrame to update transform: translateY() on images.

Robot uses a stop threshold (pixel value).

Title moves slower (speed factor < 1), robot moves faster (speed factor > 1).

5.3 Sprite Swap Logic

Exclamation + smiley images swapped with setInterval(1000ms).

Runs only when robot has settled.

6. Success Criteria

✅ Title is always the first thing users see.

✅ Robot scrolls faster, stops at defined dead stop.

✅ Exclamation fades in, animates blocky at 1 fps.

✅ Smiley swaps frames and floats.

✅ Works on desktop + mobile.

✅ Graceful fallback if reduced motion is enabled.

7. Future Enhancements

Add text overlay (team slogan).

Interactive features (e.g., hover-triggered sprite changes).

Background audio toggle.

Extend to trigger gallery scroll after animation.