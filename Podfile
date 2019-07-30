# Uncomment the next line to define a global platform for your project
platform :ios, '9.0'

pre_install do |installer|
  Pod::Installer::Xcode::TargetValidator.send(:define_method, :verify_no_static_framework_transitive_dependencies) {}
end

target 'NewHostApp' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!
  flutter_application_path = '../NewHostApp/new_flutter_module/'
  eval(File.read(File.join(flutter_application_path, '.ios', 'Flutter', 'podhelper.rb')), binding)
  # Pods for NewHostApp

  target 'NewHostAppTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'NewHostAppUITests' do
    inherit! :search_paths
    # Pods for testing
  end

end
