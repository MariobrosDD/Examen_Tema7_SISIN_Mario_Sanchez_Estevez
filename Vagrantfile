Vagrant.configure("2") do |config|
 
  config.vm.box = "ubuntu/xenial64"
  config.vm.hostname = "mario-sanchez"
 
  config.vm.provision "shell", inline: <<-SHELL
  echo "-- Insertar datos de ejemplo en la tabla 'menu' " > /home/vagrant/datos_menu.sql
    echo "INSERT INTO gestion_restaurante.menu (idPlato, nombre, descripcion, precio, categoria) VALUES" >> /home/vagrant/datos_menu.sql
    echo "(1, 'Pollo Tikka Masala', 'Pollo al estilo indio', 21.34, 'Platos exoticos')," >> /home/vagrant/datos_menu.sql
    echo "(2, 'Carrilleras al Pedro Ximenez', 'Carilleras que se deshacen', 25.99, 'popular en zamora')," >> /home/vagrant/datos_menu.sql
    echo "(3, 'Calcots a la parrilla', 'Turistada del quince para guiris', 5.27, 'rabanos asados')," >> /home/vagrant/datos_menu.sql
    


 
  SHELL
end