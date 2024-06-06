# Mi configuracion de vim

# pasos:

   *  copiar el archivo vimrc como .vimrc en la carpeta home/usuario
   * instalar plug-vim ( https://github.com/junegunn/vim-plug  )
    
        curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim

    * Instalar los plugins en .vimrc
        
        :source %
        :PlugInstall

    * Instalar Coc.vim ( https://github.com/neoclide/coc.nvim  ) (necesita nodejs >= 16.18.0)
    
        Instalar los lenguajes que se quieran soportar como:
        
        :CocInstall coc-sh        " Para Bash scripting
        :CocInstall coc-python    " Para Python
        :CocInstall coc-rls       " Para Rust (utiliza Rust Language Server)
        :CocInstall coc-tsserver  " Para JavaScript y TypeScript (utiliza TypeScript language server)
        :CocInstall coc-html      " Para HTML
        :CocInstall coc-css       " Para CSS

    * Cargar cambios
        
        :source %

