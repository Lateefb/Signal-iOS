platform :ios, '8.0'
source 'https://github.com/CocoaPods/Specs.git'

target 'Signal' do
    pod 'ATAppUpdater'
    pod 'AxolotlKit',                 git: 'https://github.com/WhisperSystems/SignalProtocolKit.git'
    #pod 'AxolotlKit',                 path: '../SignalProtocolKit'
    pod 'JSQMessagesViewController',  git: 'https://github.com/WhisperSystems/JSQMessagesViewController.git', branch: 'mkirk/retain-keyboard-view'
    #pod 'JSQMessagesViewController',   path: '../JSQMessagesViewController'
    pod 'PureLayout'
    pod 'Reachability'
    #pod 'SignalServiceKit',           git: 'https://github.com/WhisperSystems/SignalServiceKit.git'
    pod 'SignalServiceKit',           path: '../SignalServiceKit'
    pod 'SocketRocket',               :git => 'https://github.com/facebook/SocketRocket.git'
    target 'SignalTests' do
        inherit! :search_paths
    end
end

# Tests won't pass unless this is uncommented. 
#
# post_install do |installer|
#   installer.pods_project.targets.each do |target|
#     if target.to_s == "SignalServiceKit"
#       puts "--[!] Disabling singleton enforcement for SSK."
#       target.build_configurations.each do |config|
#         existing_definitions = config.build_settings['GCC_PREPROCESSOR_DEFINITIONS']
#         if existing_definitions == nil || existing.length == 0
#           existing_definitions = "$(inheritied)"
#         end
#
#         config.build_settings['GCC_PREPROCESSOR_DEFINITIONS'] = "#{existing_definitions} SSK_BUILDING_FOR_TESTS=1"
#         config.build_settings['OTHER_SWIFT_FLAGS'] = ['$(inherited)', '-DSSK_BUILDING_FOR_TESTS']
#       end
#     end
#   end
# end
