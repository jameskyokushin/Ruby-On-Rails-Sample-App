SampleApp::Application.routes.draw do
  resources :sessions, only: [:new, :create, :destroy]
  resources :users  
  
  match '/signup',  to: 'users#new'
  match '/signin',  to: 'sessions#new'
  match '/signout', to: 'sessions#destroy', via: :delete

  match '/help',    to: 'static_pages#help'
  match '/about',   to: 'static_pages#about'
  match '/contact', to: 'static_pages#contact'
  root to: 'static_pages#home'
end
