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
    pod 'SignalServiceKit',           git: 'https://github.com/WhisperSystems/SignalServiceKit.git'
    #pod 'SignalServiceKit',           path: '../SignalServiceKit'
    pod 'SocketRocket',               :git => 'https://github.com/facebook/SocketRocket.git'
    target 'SignalTests' do
        inherit! :search_paths
    end
end
