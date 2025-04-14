# Shakespeare Poem Generation with TensorFlow 🎭📜

Welcome to the magical world of Shakespearean poetry generation! Ever wanted to write like the Bard? Fear not, for we have unleashed the power of **TensorFlow** to bring forth a neural network that crafts poetry as if Shakespeare himself whispered it into existence! ✍️✨

## What Does This Do? 🤔

This project trains a TensorFlow neural network on Shakespeare's text. Using just **40 random letters** as the starting point, the model predicts the next letters, crafting poetic verses that would make even the Elizabethans proud. You can control the **length** of the text and the **temperature** (a.k.a. randomness) to fine-tune the style of the generated poetry.

## How Does It Work? 🧠

Our neural network is built using **LSTM (Long Short-Term Memory)** layers and **Dense layers**, among other TensorFlow goodies. Here's a high-level overview of the steps involved:

1. **Input Preparation**:
   - The Bard's works are tokenized, sliced, and diced into sequences of **40 characters** each.
   - Each sequence uses a **step size of 3**, meaning we move 3 characters forward to create the next training sample.

2. **Model Architecture**:
   - **LSTM Layer**: Because poetry is all about remembering the flow!
   - **Dense Layer**: For decoding the LSTM's musings into specific letters.
   - TensorFlow makes all of this as easy as reciting "To be, or not to be."

3. **Training**:
   - The model learns the intricate dance of Shakespearean prose by minimizing its letter-prediction errors.
   - After some epochs (and maybe a cup of tea), the model becomes a poetic maestro.

4. **Generation**:
   - Provide **40 random letters** as the starting sequence.
   - Set a **length** for the desired poem and adjust the **temperature** to control creativity:
     - Low temperature = more predictable, structured text.
     - High temperature = wild, avant-garde poetry.

## Installation ⚙️

Before diving into the poetic abyss, you'll need to set up your environment:

1. Clone this repository:
   ```bash
   git clone https://github.com/Narayan-cpu/shakespeare_poem_Generation.git
   cd shakespeare_poem_Generation
   ```

2. Install the required Python libraries:
   ```bash
   pip install tensorflow numpy
   ```

3. Grab a cup of coffee while TensorFlow gets cozy in your environment. ☕

## Running the Model 🚀

1. Train the Model:
   ```bash
   python train_model.py
   ```
   (This will take some time, depending on your hardware. Don't worry, the Bard rewards patience.)

2. Generate Your Poem:
   ```bash
   python generate_poem.py
   ```
   Customize the poem's **length** and **temperature** in the script to unleash your creative spirit!

## Example Output 🎉

Here’s a sample of what the model might generate after training:

> "O gentle wind, dost thou whisper soft,  
> Thy breath a melody aloft.  
> The stars doth gleam, a radiant hue,  
> In night's embrace, a dream anew."

(Okay, the model might throw in some gibberish at times, but that's part of the charm!)

## Why TensorFlow? 🤓

TensorFlow is a powerful open-source library for machine learning and deep learning. It makes building, training, and deploying neural networks easy, even for those who are new to the field. Here's why we love TensorFlow:
- **Ease of Use**: High-level APIs like Keras make it beginner-friendly.
- **Flexibility**: Allows for complex model architectures, like our LSTM-powered poet.
- **Community Support**: Tons of tutorials, forums, and resources to help you on your ML journey.

## Learnings and Takeaways 📚

- **Sequence Length Matters**: Picking the right sequence length (40 in our case) is crucial for capturing context without overloading the model.
- **Temperature is Key**: Experimenting with temperature can dramatically change the tone and creativity of the generated text.
- **Patience is Virtue**: Training a model on Shakespeare's text takes time, but the results are worth it!

## Contributing 💡

Feel inspired to improve this project? Have a better way to rhyme with "orange"? Open a pull request or start a discussion! Contributions and feedback are always welcome.

dataset :https://storage.googleapis.com/download.tensorflow.org/data/shakespeare.txt

Now, go forth and generate poetry that even Shakespeare himself would envy. Happy coding and may the Bard be with you! 🪶
