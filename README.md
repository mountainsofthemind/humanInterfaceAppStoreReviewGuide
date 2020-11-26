# humanInterfaceAppStoreReviewGuide

<!---
This repository contains a general review of the articles from "https://developer.apple.com/design/human-interface-guidelines/ios/overview/themes/" &amp; "https://developer.apple.com/app-store/review/guidelines/"
<!---
Apple Store Review Guidelines
A summary of the rules taken from "https://developer.apple.com/app-store/review/guidelines/"
Introduction
	• Guiding Principle in App Store
		○ Safe User Experience 
		○ Great opportunity for Devs to be successful
	• App must comply with ad networks, analytics services, & third-party SDKs
	• Entitlements are given in special cases
		○ Ex CarPlay Audio, HyperVisor, Privileged File Operations
			§ Review docs @developer.apple.com to learn more
	• Make sure you follow this checklist before submitting
		○ Test for crashes/bugs
		○ Complete/accurate metadata
		○ Up to date contact info
		○ Provide active demo account/login info + anything else that may be needed for app review
			§ Ex. Login credentials/sample QR Code
		○ Backend services accessible during review
		○ Includes detailed explanations in App review notes for
			§ Non-obvious features
			§ In-app purchases
			§ Supporting documentation where appropriate
		○ App follows guidance in 
			§ Dev Guidelines
				□ UIKit
				□  Appkit,
				□ WatchKit
				□  App Extensions 
				□ iOS Data Storage Guidelines
				□ Apple File System
				□ App Store Connect Help
				□ Developer Account Help
			§ Design Guidelines
				□ Human Interface Guidelines
			§ Brand & Marketing Guidelines
				□ Marketing Resources & Identity Guidelines
				□ Apple Pay Marketing Guidelines
				□ Add to Apple Wallet Guidelines
				□ Guidelines for Using Apple Trademarks & Copyrights
Safety
	• Objectionable Contend
		○ Content that's offensive, insensitive, upsetting, intended to disgust, poor taste, creepy
	• User Generated Content
		○ Apps w/user generated content or services must include
			§ Method to filter objectionable material from being posted to app
			§ Mechanism to report offensive content & timely responses to concerns
			§ Ability to block abusive users from service
			§ Published contact info so users can easily reach you
	• Kids Category
		○ A way for people to find apps for children
			§ Must not include
				□ Links outside of app
				□ Purchasing opportunities
				□ Learn about parental gates
				□ Review Privacy section to follow global privacy laws concerning children's content
				□ May not send personally identifiable information or device info to third parties
	• Physical Harm
		○ The app in no way should risk physical harm
			§ Ex: Medical apps that provide inaccurate info
			§ Drug dosage calculators must come from
				□ The drug manufacturer
				□ A hospital
				□ University
				□ Pharmacy
				□ Health Insurance Company
				□ Other approved entity
					® Or receive approval by
						◊ FDA
						◊ Or its international counterpart
		○ The app should not
			§ Encourage consumption of tobacco/vape products/illegal drugs/excessive alcohol
				□ Encourage minors to consume any of above
				□ Facilitate sale of marijuana, tobacco, or controlled substances (except for licensed pharmacies)
				□ Urge customers to participate in activities such as bets, challenges, etc
	• Developer Info
		○ Contact info published
		○ Include support URL
	• Data Security
		○ Implement appropriate security measures in app 
Performance
	• App Completeness
	• Beta Testing
	• Accurate Metadata
		○ Description, screenshots, & previews accurately reflect app's core experience 
			§ Keep up-to-date metadata w/new versions
		○ Do not include
			§ Hidden
			§ Dormant
			§ Undocumented features
		○ Describe all new features in notes
	• Hardware compatibility
		○ To ensure people get the most out of your app, iPhone apps should run on iPad when possible
			§ Consider building "universal apps" so customers can use them on all of their devices
		○ App uses power efficiently
			§ Make the code slick
	• Software Requirements
		○ Apps may only use public APIs
		○ Must run on currently shipping OS
		○ Apps should be self contained in their bundles
			§ May not read or write data outside the designated container area
		○ Multitasking apps may only use background services for their intended purposes
			§ VoIP, audio playback, location, task completion, local notifications, etc. 
				□ If app uses location background mode Include reminder that doing so may dramatically decrease battery life
		○ Apps must be fully functional on IPv6-only networks. 
		○ Apps that browse the web must use the appropriate WebKit framework & WebKit Javascript
		○ Apps using facial recognition for account authentication must use "LocalAuthentication" (& not ARKit or other facial recognition technology) where possible, & must use an alternate auth method for users under 13 years old
		○ Apps must request consent & provide clear visual &/or audio indication when recording, logging, or otherwise recording user activity.
			§ Includes use of camera, microphone, screen recordings, or other user inputs
		○ Apps that enable users to view & select files should include items from the Files app & the user's iCloud documents
Business
	• If your business model is not obvious make sure to explain in its metadata & app review notes
		○ If apple can't understand how app works, or in app purchases aren't immediately obvious, it will delay your review
		○ Follow guidelines for in-app purchases
Legal
	• Privacy
		○ Protecting user privacy is paramount in the Apple Ecosystem
		○ Must include link to privacy policy 
	• Data Use & Sharing
		○ Must obtain permission unless otherwise permitted
		○ Do not contact users w/information gathered
	• Health & Health Research
		○ Apps can't use or disclose to third parties data gathered in the health, fitness, & medical research context
		○ Must not write false or inaccurate data into HealthkKit or other similar app
		○ Must secure approval from independent ethics review board
	• Kids
		○ Must compy w/children's online privacy protection act ("COPPA"), & other appicable laws
	• Developer code of conduct
		○ Treat everyone w/respect 
    
    
    Human Interface Guidelines
  
<!--- A summary of this article taken from "https://developer.apple.com/design/human-interface-guidelines/ios/overview/themes/"
IOS
	• Themes (Ios Design Themes
		○ Clarity: Legible text, easy to understand what is what
		○ Deference: Fluid motion, content typically fills entire screen, subtle use of bezels, gradient, & shadows
		○ Depth: Hierarchy, functionality, layered content
	• Design Principles
		○ Aesthetic Integrity
			§ How well appearance works w/functionality
		○ Consistency
			§ Implements familiar standards & models (text, icons, terms, behaves in the way people would expect)
		○ Direct Manipulation
			§ Rotation of device is responsive, it has to do things when you use the app
		○ Feedback
			§ Provides for feedback response to each section, uses progress indicators for long running operations. Animation & sound clarify results of actions
		○ Metaphors
			§ Objects represent metaphors, sliders, toggle switches, etc. 
		○ User Control
			§ Suggests course of action, warns about dangerous courses of action. Generally not good for app to take over decision making. 
			§ Balance between user control, & desired outcome.
			§ Easy to cancel operations 
Interface Essentials
• Most iOS apps build using components from UIKit
	• Programming Framework
		○ Defines common interface elements. 
	• Bars
		○ Tell people where they are in your app
		○ Provide Navigation
		○ May contain buttons or other elements for initiating actions & communicating information
	• Views
		○ Contain primary content of app
			§ Text, graphics, animations, interactive elements
		○ Can enable behaviors
			§ Scrolling, insertion, deletion, & arrangement
	• Controls
		○ Initiate actions, convey info
		○ Ex. Buttons, switches, text fields, progress indicators
Launching
• Provide Launch Screen
	• Works Quickly & efficiently
	• Correct Orientation
• Don't ask for setup info up front
• Don't show in-app license agreements & disclaimers
• Restore previous state when app restarts
• Don't encourage reboots
• Don't ask for ratings too often
Onboarding
• Lets you welcome new users & reconnect w/returning ones
• Avoid including setup or licensing details in your onboarding experience
	• See Launching
• Get to the point
	• If you need intro features, allow option to skip it
• Anticipate need for help
	• Proactively look for times people might get stuck
• Stick to the essentials in tutorials
	• If too much guidance is needed revisit the app design
	• Learning by doing is more fun & effective then reading intro instructions
Loading
	• Make sure people understand when loading so they don't think it froze
Modality
	• A Design Technique
		○ Presents content in a temp mode separate from previous context
	• EX: Alerts, 
	• Use when it makes sense, only when it is critical for functionality
Navigation
	• Make it seemless
	• Hiirarchical Navigation
		○ One choice per screen til destination is reached
	• Flat Navigation
		○ Switch between multiple content categories
			§ Ex. Music & App store
	• Content-Driven, or Experience-Driven
		○ More sophisticated design may be hybrid of other options
Requesting Permission
	• Users must grant permission for an app to access personal info
		○ Location, calendar, contact information, reminders, & photos
		○ Only request personal data if app truly needs it
		○ Explain why this info is needed
		○ Only request permission at launch if necessary for app functionality
		○ Use the system-provided alert
Settings
	• Successful apps work right away w/out adjusting settings 
	• Query system for info when possible instead of asking user
	• Ex. Ask permission to use their current location
		○ Fall back to manual entry if user denies access to the system info
	• Make config Options Follow priority
		○ Most used at front
		○ Secondary screens for config options that change only occasionally 
	• For options rarely changed
		○ See Implementing an iOS Settings Bundle
			§ In "preferences & settings Programming guide
	• Provide shortcuts to settings when appropriate
		○ Rather then directing users to "Go to settings > MyApp > Privacy > Location Services"
			§ Add a button that opens that location automatically for users
				□ See opensettingsURLString in UIApplication

--->

	


	



