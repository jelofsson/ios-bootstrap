# iOS Bootstrap

My personal WIKI how to set up a simple ios project. The idea is that I will add info about useful tools.

## CocoaPods

[CocoaPods](https://cocoapods.org/app) manages library dependencies for your Xcode projects.
	

#### Installation

	sudo gem install cocoapods

#### Useful Pods

[AFNetworking](https://cocoapods.org/pods/AFNetworking)
[MagicalRecord](https://cocoapods.org/pods/MagicalRecord)

####[Podfile](https://guides.cocoapods.org/syntax/podfile.html) example
	
	# open source
	source 'https://github.com/CocoaPods/Specs.git'
	
	pod 'AFNetworking', '~> 2.0'
	pod 'MagicalRecord', '~> 1.0'
	
	target 'MyApp' do
		pod 'AFNetworking'
	end


	
## Project folder structure

	ProjectName  
    |-Assets
    |---Images
    |-Frameworks
    |-Logic
    |---Models
    |-Presentation
    |---ViewControllers
    |---Views

#### Command for creating the project folders

	mkdir -p ProjectName/{Assets/Images,Frameworks,Logic/Models,Presentation/View{,Controller}s}

#### synx
    
[synx](https://github.com/venmo/synx) - A command-line tool that reorganizes your Xcode project folder to match your Xcode groups