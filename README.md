# humanInterfaceAppStoreReviewGuide


This repository contains a general review of the articles from "https://developer.apple.com/design/human-interface-guidelines/ios/overview/themes/" &amp; <br>"https://developer.apple.com/app-store/review/guidelines/"<br>
Apple Store Review Guidelines<br>
A summary of the rules taken from "https://developer.apple.com/app-store/review/guidelines/"<br>
Introduction <br>
	• Guiding Principle in App Store <br>
		○ Safe User Experience <br>
		○ Great opportunity for Devs to be successful<br>
	• App must comply with ad networks, analytics services, & third-party SDKs<br>
	• Entitlements are given in special cases<br>
		○ Ex CarPlay Audio, HyperVisor, Privileged File Operations<br>
			§ Review docs @developer.apple.com to learn more<br>
	• Make sure you follow this checklist before submitting<br>
		○ Test for crashes/bugs<br>
		○ Complete/accurate metadata<br>
		○ Up to date contact info<br>
		○ Provide active demo account/login info + anything else that may be needed for app review<br>
			§ Ex. Login credentials/sample QR Code<br>
		○ Backend services accessible during review<br>
		○ Includes detailed explanations in App review notes for<br>
			§ Non-obvious features<br>
			§ In-app purchases<br>
			§ Supporting documentation where appropriate<br>
		○ App follows guidance in <br>
			§ Dev Guidelines<br>
				□ UIKit<br>
				□  Appkit,<br>
				□ WatchKit<br>
				□  App Extensions <br>
				□ iOS Data Storage Guidelines<br>
				□ Apple File System<br>
				□ App Store Connect Help<br>
				□ Developer Account Help<br>
			§ Design Guidelines<br>
				□ Human Interface Guidelines<br>
			§ Brand & Marketing Guidelines<br>
				□ Marketing Resources & Identity Guidelines<br>
				□ Apple Pay Marketing Guidelines<br>
				□ Add to Apple Wallet Guidelines<br>
				□ Guidelines for Using Apple Trademarks & Copyrights<br>
Safety<br>
	• Objectionable Content<br>
		○ Content that's offensive, insensitive, upsetting, intended to disgust, poor taste, creepy<br>
	• User Generated Content<br>
		○ Apps w/user generated content or services must include<br>
			§ Method to filter objectionable material from being posted to app<br>
			§ Mechanism to report offensive content & timely responses to concerns<br>
			§ Ability to block abusive users from service<br>
			§ Published contact info so users can easily reach you<br>
	• Kids Category<br>
		○ A way for people to find apps for children<br>
			§ Must not include<br>
				□ Links outside of app<br>
				□ Purchasing opportunities<br>
				□ Learn about parental gates<br>
				□ Review Privacy section to follow global privacy laws concerning children's content<br>
				□ May not send personally identifiable information or device info to third parties<br>
	• Physical Harm<br>
		○ The app in no way should risk physical harm<br>
			§ Ex: Medical apps that provide inaccurate info<br>
			§ Drug dosage calculators must come from<br>
				□ The drug manufacturer<br>
				□ A hospital<br>
				□ University<br>
				□ Pharmacy<br>
				□ Health Insurance Company<br>
				□ Other approved entity<br>
					® Or receive approval by<br>
						◊ FDA<br>
						◊ Or its international counterpart<br>
		○ The app should not<br>
			§ Encourage consumption of tobacco/vape products/illegal drugs/excessive alcohol<br>
				□ Encourage minors to consume any of above<br>
				□ Facilitate sale of marijuana, tobacco, or controlled substances (except for licensed pharmacies)<br>
				□ Urge customers to participate in activities such as bets, challenges, etc<br>
	• Developer Info<br>
		○ Contact info published<br>
		○ Include support URL<br>
	• Data Security<br>
		○ Implement appropriate security measures in app <br>
Performance<br>
	• App Completeness<br>
	• Beta Testing<br>
	• Accurate Metadata<br>
		○ Description, screenshots, & previews accurately reflect app's core experience <br>
			§ Keep up-to-date metadata w/new versions<br>
		○ Do not include<br>
			§ Hidden<br>
			§ Dormant<br>
			§ Undocumented features<br>
		○ Describe all new features in notes<br>
	• Hardware compatibility<br>
		○ To ensure people get the most out of your app, iPhone apps should run on iPad when possible<br>
			§ Consider building "universal apps" so customers can use them on all of their devices<br>
		○ App uses power efficiently<br>
			§ Make the code slick<br>
	• Software Requirements<br>
		○ Apps may only use public APIs<br>
		○ Must run on currently shipping OS<br>
		○ Apps should be self contained in their bundles<br>
			§ May not read or write data outside the designated container area<br>
		○ Multitasking apps may only use background services for their intended purposes<br>
			§ VoIP, audio playback, location, task completion, local notifications, etc.<br> 
				□ If app uses location background mode Include reminder that doing so may dramatically decrease battery life<br>
		○ Apps must be fully functional on IPv6-only networks. <br>
		○ Apps that browse the web must use the appropriate WebKit framework & WebKit Javascript<br>
		○ Apps using facial recognition for account authentication must use "LocalAuthentication" (& not ARKit or other facial recognition technology) <br>where possible, & must use an alternate auth method for users under 13 years old<br>
		○ Apps must request consent & provide clear visual &/or audio indication when recording, logging, or otherwise recording user activity.<br>
			§ Includes use of camera, microphone, screen recordings, or other user inputs<br>
		○ Apps that enable users to view & select files should include items from the Files app & the user's iCloud documents<br>
Business<br>
	• If your business model is not obvious make sure to explain in its metadata & app review notes<br>
		○ If apple can't understand how app works, or in app purchases aren't immediately obvious, it will delay your review<br>
		○ Follow guidelines for in-app purchases<br>
Legal<br>
	• Privacy<br>
		○ Protecting user privacy is paramount in the Apple Ecosystem<br>
		○ Must include link to privacy policy <br>
	• Data Use & Sharing<br>
		○ Must obtain permission unless otherwise permitted<br>
		○ Do not contact users w/information gathered<br>
	• Health & Health Research<br>
		○ Apps can't use or disclose to third parties data gathered in the health, fitness, & medical research context<br>
		○ Must not write false or inaccurate data into HealthkKit or other similar app<br>
		○ Must secure approval from independent ethics review board<br>
	• Kids<br>
		○ Must compy w/children's online privacy protection act ("COPPA"), & other appicable laws<br>
	• Developer code of conduct<br>
		○ Treat everyone w/respect <br>
    
    
    Human Interface Guidelines<br>
  
 A summary of this article taken from "https://developer.apple.com/design/human-interface-guidelines/ios/overview/themes/"<br>
IOS<br>
	• Themes (Ios Design Themes<br>
		○ Clarity: Legible text, easy to understand what is what<br>
		○ Deference: Fluid motion, content typically fills entire screen, subtle use of bezels, gradient, & shadows<br>
		○ Depth: Hierarchy, functionality, layered content<br>
	• Design Principles<br>
		○ Aesthetic Integrity<br>
			§ How well appearance works w/functionality<br>
		○ Consistency<br>
			§ Implements familiar standards & models (text, icons, terms, behaves in the way people would expect)<br>
		○ Direct Manipulation<br>
			§ Rotation of device is responsive, it has to do things when you use the app<br>
		○ Feedback<br>
			§ Provides for feedback response to each section, uses progress indicators for long running operations. Animation & sound clarify results of actions<br>
		○ Metaphors<br>
			§ Objects represent metaphors, sliders, toggle switches, etc. <br>
		○ User Control<br>
			§ Suggests course of action, warns about dangerous courses of action. Generally not good for app to take over decision making. <br>
			§ Balance between user control, & desired outcome.<br>
			§ Easy to cancel operations <br>
Interface Essentials<br>
• Most iOS apps build using components from UIKit<br>
	• Programming Framework<br>
		○ Defines common interface elements. <br>
	• Bars<br>
		○ Tell people where they are in your app<br>
		○ Provide Navigation<br>
		○ May contain buttons or other elements for initiating actions & communicating information<br>
	• Views<br>
		○ Contain primary content of app<br>
			§ Text, graphics, animations, interactive elements<br>
		○ Can enable behaviors<br>
			§ Scrolling, insertion, deletion, & arrangement<br>
	• Controls<br>
		○ Initiate actions, convey info<br>
		○ Ex. Buttons, switches, text fields, progress indicators<br>
Launching<br>
• Provide Launch Screen<br>
	• Works Quickly & efficiently<br>
	• Correct Orientation<br>
• Don't ask for setup info up front<br>
• Don't show in-app license agreements & disclaimers<br>
• Restore previous state when app restarts<br>
• Don't encourage reboots<br>
• Don't ask for ratings too often<br>
Onboarding<br>
• Lets you welcome new users & reconnect w/returning ones<br>
• Avoid including setup or licensing details in your onboarding experience<br>
	• See Launching<br>
• Get to the point<br>
	• If you need intro features, allow option to skip it<br>
• Anticipate need for help<br>
	• Proactively look for times people might get stuck<br>
• Stick to the essentials in tutorials<br>
	• If too much guidance is needed revisit the app design<br>
	• Learning by doing is more fun & effective then reading intro instructions<br>
Loading<br>
	• Make sure people understand when loading so they don't think it froze<br>
Modality<br>
	• A Design Technique<br>
		○ Presents content in a temp mode separate from previous context<br>
	• EX: Alerts, <br>
	• Use when it makes sense, only when it is critical for functionality<br>
Navigation<br>
	• Make it seemless<br>
	• Hiirarchical Navigation<br>
		○ One choice per screen til destination is reached<br>
	• Flat Navigation<br>
		○ Switch between multiple content categories<br>
			§ Ex. Music & App store<br>
	• Content-Driven, or Experience-Driven<br>
		○ More sophisticated design may be hybrid of other options<br>
Requesting Permission<br>
	• Users must grant permission for an app to access personal info<br>
		○ Location, calendar, contact information, reminders, & photos<br>
		○ Only request personal data if app truly needs it<br>
		○ Explain why this info is needed<br>
		○ Only request permission at launch if necessary for app functionality<br>
		○ Use the system-provided alert<br>
Settings<br>
	• Successful apps work right away w/out adjusting settings <br>
	• Query system for info when possible instead of asking user<br>
	• Ex. Ask permission to use their current location<br>
		○ Fall back to manual entry if user denies access to the system info<br>
	• Make config Options Follow priority<br>
		○ Most used at front<br>
		○ Secondary screens for config options that change only occasionally <br>
	• For options rarely changed<br>
		○ See Implementing an iOS Settings Bundle<br>
			§ In "preferences & settings Programming guide<br>
	• Provide shortcuts to settings when appropriate<br>
		○ Rather then directing users to "Go to settings > MyApp > Privacy > Location Services"<br>
			§ Add a button that opens that location automatically for users<br>
				□ See opensettingsURLString in UIApplication<br>



	


	



