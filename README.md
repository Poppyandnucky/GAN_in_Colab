# GAN_in_Colab
When importing keras.optimizers.Adam in colab, we may encounter some problems. This is due to the version and API has been conflicting with keras 3. By applying such import command we can successfully import the libraries:
instead of:
from tensorflow.keras.optimizer import Adam
we use:
opt = keras.optimizers.Adam(learning_rate=0.00005, beta_1=0.5)
