class profile::ssh_server {
  package {'openssh-server':
    ensure => present,
  }
  service { 'sshd':
    ensure => 'running',
    enable => 'true',
  }
  ssh_authorized_key { 'root@master.puppet.vm':
    ensure => present,
    user   => 'root',
    type   => 'ssh-rsa',
    key    => 'AAAAB3NzaC1yc2EAAAADAQABAAABAQC2cDUCsPVB/g0YgWD50ITq6uvr1kphqsmV9jh6TfT37c2iDXoIONx8YNODSjSQugcqGHgGa2VCfO07JUx/qIDhZTbp9hBKE22+nO7NprOZVetfW2LxfgipVx/+DziqtjtNlK+LOxeJ77eLNDvn9B1H5V9w59NTiERF3R8k1sO7Httb3fXhOhJePDPCRAbzt3UvKdDXglghrm4sDmmKtd+rVbPjRn5JFw2Uf0/XCEy5bnqe2ZIhoHmHGiHPGj4OMgy1eVHyHj1Oi5AcjMBAi9ueHVN5IAhzTEFNeHd3YwrlG4gUrInJcjY2aNOlfbYyfyjtbByKObXr9UWP3dWSwNBJ',
  }  
}
