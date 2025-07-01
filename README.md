# emacs-theme-vim
Emacs theme that mimics Vim's default colorscheme.

<img width="1552" alt="image" src="https://github.com/user-attachments/assets/0cc4c6fd-ac7f-4ca6-aeca-920d2fbfd715" />

To use, add the following snippet to your  `.emacs` file or `.emacs.d/init.el`.
```
(add-hook 'prog-mode-hook                                                                                                         
          (lambda ()                                                                                                              
            (font-lock-add-keywords                                                                                               
             nil                                                                                                                  
             '(("\\_<[0-9]+\\(?:\\.[0-9]+\\)?\\_>"  ; integers & floats                                                           
                0 'font-lock-number-face keep)))))                                                                                
                                                                                                                                  
;; ~/.emacs or init.el                                                                                                            
(add-to-list 'custom-theme-load-path                                                                                              
             (expand-file-name "themes" user-emacs-directory))                                                                    
(load-theme 'my-vim-mac t)      ; ‘t’ = load w/o query                                                                            
(custom-set-variables)
(custom-set-faces '(font-lock-number-face ((t (:foreground "#EC4FF7"))))) 
```
