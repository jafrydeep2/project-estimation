# Project Review: Observations & Suggestions

Hello,

After spending some time digging into the codebase, I wanted to share my honest thoughts to make the project even better. Here's what stood out to me:

---

## Issues

### 1. Large Screens
A few screens (like SocialScreen.js and PostDetails.js) have grown into huge files that try to do too much at once. When one file handles everything from UI to data fetching to business logic, it becomes a pain to update or debug. If something breaks, it can take ages to track down the problem.

### 2. Folder Structure
There are folders with almost the same name (like `navigation` and `navigations`), and some code is in `src/` while other bits are in `app/`. It's not always clear where to look for things, which can be frustrating.

### 3. State Management
Right now, the app uses React Context for sharing data between screens. That's fine for smaller projects, but as things grow, it can get tricky to keep everything in sync and avoid weird bugs.

### 4. Large API File
Most of the code that talks to the backend is in a single, very large file. This means if two people want to work on different features, they might get in each other's way.

### 5. Utilities
Some files that store images, constants, or helper functions have gotten pretty big. It's easy to lose track of what's in there, and updating them can feel risky.

### 6. Not Enough Automated Tests
There's some setup for automated testing, but it's not clear if the most important parts of the app are actually covered. This means bugs could sneak through without us noticing.

### 7. TypeScript
The project is set up for TypeScript (which helps catch errors before they happen), but most files are still plain JavaScript.
I think it's a good idea to start using TypeScript gradually, so we can catch mistakes before they become real problems.

### Additional Issues and Suggestions

#### Asset Management
- **Image Organization**: The `src/assets/images` directory contains a large number of image files, which may lead to maintenance challenges. 
- **Button Images**: The `src/assets/buttons` directory has multiple button images. Evaluate if these can be replaced with styled components or SVG icons to reduce the number of assets.
- **Video Content**: The `src/assets/video` directory contains a tutorial video. Ensure that video content is optimized for mobile devices to reduce load times and bandwidth usage.

#### Font Management
- **Font Files**: The `src/assets/fonts` directory includes multiple font files. Consider using a font loading strategy to improve performance and reduce the initial load time.

#### Power Level and Notifications
- **Power Level Images**: The `src/assets/images/powerLevel` directory contains numerous images for different power levels. 
- **Notification Images**: The `src/assets/images/notifications` directory has various notification icons. 
Need to check if we can use icons/components instead of images to improve performance and reduce the number of assets.

#### Onboarding and Tutorials
- **Onboarding Images**: The `src/assets/images/onboard` directory contains multiple onboarding images. 
Need to check if we can use icons/components instead of images to improve performance and reduce the number of assets.

---

## Suggestions

1. **Break Up the Biggest Screens**
   - Let's split the huge screens into smaller, focused components. This will make them easier to work on and test.

2. **Tidy Up the Folder Structure**
   - We should pick one main folder for the code and merge or rename any confusingly similar folders. This will make the project feel less chaotic.

3. **Upgrade State Management**
   - As the app grows, it might be worth moving to something like Redux Toolkit or Zustand. These tools are built for bigger projects and can help keep things organized.

4. **Split Up the API Code**
   - Organize backend-related code by feature, so different people can work on different things without stepping on each other's toes.

5. **Break Down Utility Files**
   - Let's split up the big utility files so each one has a clear purpose.

6. **Add More Automated Tests**
   - Focus on testing the most important features first. This will help us catch bugs early and make releases less stressful.

7. **Start Using TypeScript Gradually**
   - We don't have to do it all at once, but converting files to TypeScript over time will help us catch mistakes before they become real problems.

8. **Optimize Asset Management**
   - Reorganize images into logical subdirectories and convert button images to styled components or SVGs
   - Implement a font loading strategy to improve performance
   - Optimize and standardize notification and power level icons
   - Enhance onboarding experience with optimized images and carousel components


---

## Rough Timeline

| Task                        | Estimated Time     |
|-----------------------------|--------------------|
| Refactor large screens      | 2-3 weeks          |
| Clean up folder structure   | 2-3 days           |
| Upgrade state management    | 1 week             |
| Split up API code           | 1 week             |
| Organize utility files       | 3-4 days           |
| Improve automated testing   | 1 week             |
| Adopt TypeScript            | 2 weeks (ongoing)  |
| Asset optimization          | 1 week             |

Some of these can happen at the same time, so we don't have to do them all in order.
It's an approximate timeline, and we can adjust it based on the project's needs. Since few things will be done at once, I think we can complete all of them in 4 weeks.

Happy to chat through any of these points or adjust the plan based on what's most important to you. Just let me know what you think!

Thank You

Best Regards,

Jafry Mondol Deep
