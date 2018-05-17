# ULL Practical 2

We provide our notebooks for Skip-gram, Bayesian Skip-gram and Embed-Align. Along with these, we submit the code for performing the Lexical subsititution task and GAP evaluation for each model and AER evaluation for Embed-Align. We also provide our code for generating data for skip-gram that creates positive samples and negative samples. For Embed-Align, we apply a different procedure to preprocess the data.


## Libraries
import numpy as np

from scipy.stats import pearsonr
from scipy.stats import spearmanr
from sklearn.metrics.pairwise import cosine_similarity
from scipy import spatial
from scipy import stats

import torch
from torch.autograd import Variable
import torch.nn as nn
import torch.autograd as autograd
import torch.optim as optim
import torch.nn.functional as F
torch.manual_seed(1)

import time
from datetime import datetime

from collections import defaultdict
from collections import Counter

from random import randint
import pickle

import warnings
warnings.filterwarnings('error')

from sklearn.metrics.pairwise import cosine_similarity
from scipy import spatial

import string
puncs = set(string.punctuation)

import matplotlib.pyplot as plt

from sklearn.metrics.pairwise import cosine_similarity
from scipy import spatial
