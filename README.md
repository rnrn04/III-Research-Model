# III-Research-Model
Modifications made:
- Changed the classes (microorganisms) that would be tested
- Translated the notes into english
- "from google.colab import drive" has not yet been modified
  
Errors (during run and debugg sessions, here are the errors occured):
-Cell In[1], line 3
      1 # Create data loaders
      2 batch_size=128
----> 3 train_loader = DataLoader(train_set, batch_size=batch_size, shuffle=True)
      4 val_loader = DataLoader(val_set, batch_size=batch_size, shuffle=False)
      5 test_loader = DataLoader(test_set, batch_size=batch_size, shuffle=False)

NameError: name 'DataLoader' is not defined


- Cell In[3], line 16
     13   return mean, std
     15 # Calculăm media și abaterea standard pe setul de antrenament
---> 16 mean, std = compute_mean_std(train_loader)
     17 print(f'Media: {mean}')
     18 print(f'Abaterea standard: {std}')

NameError: name 'train_loader' is not defined
