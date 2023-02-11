# Deep-Learning-and-NLP-A-Z-How-to-create-a-ChatBot

End-to-end Deep Learning Models
    -- End-to-end
        -- One neural network that runs the whole show
Seq2Seq
    -- Architecture
        -- Follows a Recurrent Neural Network
            -- Utalizing Memeory
            -- A LSTM layer
        -- Encoder and Decoder
        -- Can have multiple hidden layers to put the input through
    -- Training
        -- Weights
            -- Updated normally through backpropigation like a RNN
            -- Weights are the same for every h(of n) value
        -- The model will updates weights based on the words that it has previously given
        -- The goal for the Seq2Seq is that it wants to model the logic and behavior that was observed in the email
Greedy Decoding vs Beam Search Decoding 
    -- What are the differnces
        -- Greedy
            -- It only looks at the word with the highest probibility to give an output sentence
        -- Beam
            -- It looks at the top 3 words with the highest probibility
            -- The look is like a binary tree
            -- This is similar to how autocorrect works
            -- It will throw away the options with the lowest joint probibility
            -- There are techniques to make the three outputs different
Attention Mechanisms
    -- Global attention
        -- Looking at each of the weights of importance
        -- The decoder will give weights of importance to each input
            -- The bigger the weight the higher importance
            -- Softmax function is applied
            -- Create a contex vector
                -- A weighted sum of all the different weights of importance
    -- Local attention 
        -- Similar to what humans do
        -- Only look at some of the weights of importance 