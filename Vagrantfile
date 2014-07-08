VAGRANTFILE_API_VERSION = "2"
Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.define "elasticsearch" do |v|
    v.vm.provider "docker" do |d|
      d.image = "dockerfile/elasticsearch"
      d.ports = ["9200:9200"]
      d.vagrant_vagrantfile = "./Vagrantfile.proxy"
    end
  end

end
