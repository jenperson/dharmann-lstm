# Generate text from Dhar Mann video scripts
# using an LSTM text generator model

To run this model, clone the [`tfjs-examples`](https://github.com/tensorflow/tfjs-examples)
repository.

Download the contents of the `dharmann-lstm` repository, and then add it to the `lstm-text-generation`
folder in `tfjs-examples`.

Generate text using the following commands:

```
yarn
yarn gen dharmann-scripts.txt  ./dharman-scripts-model/model.json \
    --genLength 250 \
    --temperature 0.6
```

Change the value of `genLength` to change the number of characters generated.
Change the value of `temperature` to a number between 0 and 1 to raise or
lower then randomness of the text. A higher value means the text
generated will appear more random.